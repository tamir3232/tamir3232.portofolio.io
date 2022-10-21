<script>

export default {

  name: "TestView",
  data() {
    return {
      title: "Test",
      input: {
        name: "",
        email: "",
        gender: null,
        message:"",
      },
      gender: [{ text: "Select One", value: null }, "male","female"],
    };
  },
  methods: {
    submitt() {
      console.log(JSON.stringify(this.input));
    },
  },
};</script>
<template>
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body>
        <div style="margin:250px 650px">
            <form action="">
      <BaseInput v-model="input.name" name="name" label="Name" type="text" />
      <BaseInput
        v-model="input.email"
        name="email"
        label="Email"
        type="email"
      />
      <br />
      <select v-model="input.gender">
        <option enable value="">Please select Your gender</option>
        <option>male</option>
        <option>female</option>
        
      </select>
      <BaseInput v-model="input.message" name="message" label="message" type="message" />
      <br />
      <button @click.prevent="submitt">SUBMIT</button>
    </form>
        </div>

    </body>
    </html>
</template>