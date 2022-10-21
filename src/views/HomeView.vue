<template>
  
    

    <body>
      <section class="hero">
        <div class="hero container">
          <div>
            <div>
              <img class="foto" src="../assets/tamir.png" alt="" />
            </div>
          </div>
          <div style="font-family: Arial">
            <h1 style="font-size: 70px; margin-bottom: 20px">
              HELLO <span></span>
            </h1>
            <h2 style="font-size: 30px; color: whitesmoke; margin-bottom: 5px">
              Sedikit Tentang ku <span></span>
            </h2>
            <P style="font-size: 20px; color: whitesmoke">Aku adalah seorang Back end Engineer <br />karena aku sangat
              tidak suka berurusan denga User Interface,<br />
              aku sekarang kuliah di Universitas Sumatera Utara jurusan <br />
              ILMU KOMPUTER</P>

            <router-link to="/myproject"><button>My Project</button></router-link>

            <router-link to="/Contact"><button>Contact</button></router-link>
           
          </div>
        </div>
      </section>
    </body>

   
</template>
<style>
@import url("https://fonts.googleapis.com/css2?family=Shadows+Into+Light&display=swap");
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
button,
button::after {
  width: 120px;
  height: 30px;
  background: linear-gradient(45deg, transparent 5%, #ff013c 5%);
  border: 0;
  color: #fff;
  box-shadow: 6px 0px 0px #00e6f6;
  outline: transparent;
  position: relative;
  margin-right: 30px;
}

button::after {
  --slice-0: inset(50% 50% 50% 50%);
  --slice-1: inset(80% -6px 0 0);
  --slice-2: inset(50% -6px 30% 0);
  --slice-3: inset(10% -6px 85% 0);
  --slice-4: inset(40% -6px 43% 0);
  --slice-5: inset(80% -6px 5% 0);

  content: "AVAILABLE NOW";
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(
    45deg,
    transparent 3%,
    #00e6f6 3%,
    #00e6f6 5%,
    #ff013c 5%
  );
  text-shadow: -3px -3px 0px #f8f005, 3px 3px 0px #00e6f6;
  clip-path: var(--slice-0);
}

button:hover::after {
  animation: 1s glitch;
  animation-timing-function: steps(2, end);
}

@keyframes glitch {
  0% {
    clip-path: var(--slice-1);
    transform: translate(-20px, -10px);
  }
  10% {
    clip-path: var(--slice-3);
    transform: translate(10px, 10px);
  }
  20% {
    clip-path: var(--slice-1);
    transform: translate(-10px, 10px);
  }
  30% {
    clip-path: var(--slice-3);
    transform: translate(0px, 5px);
  }
  40% {
    clip-path: var(--slice-2);
    transform: translate(-5px, 0px);
  }
  50% {
    clip-path: var(--slice-3);
    transform: translate(5px, 0px);
  }
  60% {
    clip-path: var(--slice-4);
    transform: translate(5px, 10px);
  }
  70% {
    clip-path: var(--slice-2);
    transform: translate(-10px, 10px);
  }
  80% {
    clip-path: var(--slice-5);
    transform: translate(20px, -10px);
  }
  90% {
    clip-path: var(--slice-1);
    transform: translate(-10px, 0px);
  }
  100% {
    clip-path: var(--slice-1);
    transform: translate(0);
  }
}

html {
  font-size: 10px;
  font-family: "shadows";
}

a {
  text-decoration: none;
}

.container {
  min-height: 100vh;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.hero {
  background-image: url(../assets/wall.png);
  background-size: cover;
  background-position: top center;
  position: relative;
}

.hero::after {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  height: 100%;
  width: 100%;
  background-color: black;
  opacity: 0.7;
  z-index: -1;
}

.hero h1 {
  display: block;
  width: fit-content;
  font-size: 4rem;
  position: relative;
  color: #815b5b;
}

.hero h1 span {
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 0%;
  background-color: grey;
  animation: text_reveal_box 0.5s ease;
  animation-delay: 0s;
}

.hero .cta {
  display: inline-block;
  padding: 10px 30px;
  color: white;
  background-color: transparent;
  border: 3px solid grey;
  font-size: 2rem;
  text-transform: uppercase;
  letter-spacing: 0.1rem;
  margin-top: 30px;
  transition: 0.3s ease;
  transition-property: background-color, color;
  border-radius: 10px;
}

.hero .container {
  /* max-width: 1200px; */
  margin: 0 auto;
  padding: 0 100px;
  justify-content: flex-start;
}

.hero .cta:hover {
  color: white;
  background-color: black;
}

#keahlian .keahlian {
  flex-direction: column;
  text-align: center;
  max-width: 1500px;
  margin: 0 auto;
  padding: 100px 0;
}

#keahlian .section-title {
  font-size: 4rem;
  font-weight: 300;
  color: black;
  margin-bottom: 10px;
  text-transform: uppercase;
  letter-spacing: 0.2rem;
  text-align: center;
}

#keahlian .section-title span {
  color: crimson;
}

#keahlian .keahlian-atas p {
  font-size: 1.4rem;
  margin-top: 5px;
  line-height: 2.5rem;
  font-weight: 300;
  letter-spacing: 0.05rem;
}

#keahlian .keahlian-bawah {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
}

#keahlian .keahlian-item {
  flex-basis: 80%;
  display: flex;
  align-items: flex-start;
  justify-content: center;
  flex-direction: column;
  padding: 30px;
  border-radius: 10px;
  background-image: url(../assets/arif-riyanto-1DRq1ZsE2N0-unsplash.jpg);
  background-size: cover;
  margin: 10px 5%;
  color: aliceblue;
}

#keahlian .keahlian-item::after {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  height: 100%;
  width: 100%;
}

#keahlian .keahlian-bawah .icon {
  height: 80px;
  width: 80px;
  margin: 20px;
}

#keahlian .keahlian-bawah img {
  height: 100%;
  width: 100%;
  object-fit: cover;
}

#keahlian .keahlian-item h2 {
  font-size: 2rem;
  color: white;
  margin-bottom: 10px;
  text-transform: uppercase;
}

#keahlian .keahlian-item p {
  color: white;
  text-align: left;
  font-size: 1.4rem;
  line-height: 1.9rem;
}

.foto {
  border-radius: 100%;
  background-color: grey;
  width: 70%;
  height: 60%;
  margin-right: 1px;
}

#biodata .biodata {
  flex-direction: column;
  text-align: center;
  max-width: 1000px;
  height: 10px;
  margin: 50px auto;
  margin-bottom: 20px;
  padding: 100px 0;
}

.biodata {
  flex-basis: 80%;
  display: flex;
  font-family: Arial, Helvetica, sans-serif;
  justify-content: center;
  flex-direction: column;

  border-radius: 10px;
  background-color: #150050;
  background-size: cover;
  margin: 10px 5%;
  color: aliceblue;
}

#biodata .biodata h2 {
  font-size: 2rem;
  color: white;
  margin-bottom: 10px;
  text-transform: uppercase;
  text-align: center;
}

#biodata .biodata p {
  color: white;
  text-align: center;
  font-size: 1.4rem;
  line-height: 1.9rem;
}

@keyframes text_reveal_box {
  50% {
    width: 100%;
    left: 0;
  }
  100% {
    width: 0;
    left: 100%;
  }
}
</style>
<script>
// @ is an alias to /src


export default {
  name: "HomeView",

};
</script>
