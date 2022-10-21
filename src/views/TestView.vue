<script>
import BaseInput from "../components/BaseInput.vue";
export default {
  name: "TestView",
  data() {
    return {
      title: "Test",
      input: {
        name: "",
        email: "",
        class: null,
        message:""
        
      },
      class: [{ text: "Select One", value: null }, "A", "B", "C"],
    };
  },
  components: { BaseInput },
  methods: {
    submitt() {
      console.log(JSON.stringify(this.input));
    },
  },
};
</script>
<template>
  <div class="test">
    <form action="">
      <BaseInput v-model="input.name" name="name" label="Name" type="text" />
      <BaseInput
        v-model="input.email"
        name="email"
        label="Email"
        type="email"
      />
      <br />
      <select v-model="input.class">
        <option enable value="">Please select Your Class</option>
        <option>A</option>
        <option>B</option>
        <option>C</option>
      </select>
      <BaseInput v-model="input.message" name="message" label="message" type="message" />
      
      <br />
      <button @click.prevent="submitt">SUBMIT</button>
    </form>
  </div>
</template>
<style>
@media (min-width: 1024px) {
  .test {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
