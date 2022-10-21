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
        <div class="name-project" style="margin:100px auto; margin-left: 120px;">
            <h1 style="color:aliceblue;font-family:sans-serif; font-size: 40px;">
                PROJECT</h1>  
        </div>
       <div class="project-container" style="margin:120px; font-family: Arial, Helvetica, sans-serif;">
          
        <a href="https://github.com/tamir3232/TUGAS_Bingleshop" class="card1" >
      <div class="inner">
        <h2 class="title">API ONLINE SHOP</h2>
        <time class="subtitle">25 JULI 2022</time>
      </div>
         </a>
         <a href="https://github.com/tamir3232/Website-Hotel-Menggunakan-Semantic-Web" class="card2">
      <div class="inner">
        <h2 class="title">Website hotel menggunakan RDF dan Semantic Web</h2>
        <time class="subtitle">08 JULI 2022</time>
      </div>
         </a>
         <a href="https://github.com/tamir3232/APLIKASI-KASIR-JAVA-" class="card3">
      <div class="inner">
        <h2 class="title">APLIKASI KASIR SEDERHANA</h2>
        <time class="subtitle">09 September 2021</time>
      </div>
         </a>
           

       </div>
    </body>
    </html>
</template>
<style>
body {
  background-image: url(../assets/wall.png);
  background-size: cover;
 
}

.card1 {
  height: 400px;
  position: relative;
  padding: 20px;
  box-sizing: border-box;
  display: flex;
  align-items: flex-end;
  text-decoration: none;
  border: 4px solid #b0215e;
  margin-bottom: 20px;
  background-image: url('../assets/Screenshot_17.png'); 
    background-size: cover;
  
  @include media {
    height: 500px;
  }
}

.card2 {
  height: 400px;
  position: relative;
  padding: 20px;
  box-sizing: border-box;
  display: flex;
  align-items: flex-end;
  text-decoration: none;
  border: 4px solid #b0215e;
  margin-bottom: 20px;
  background-image: url('../assets/2022-02-16-ternyata-ini-bedanya-jumlah-bintang-di-tiap-hotel.jpg'); 
    background-size: cover;
  
  @include media {
    height: 500px;
  }
}

.card3 {
  height: 400px;
  position: relative;
  padding: 20px;
  box-sizing: border-box;
  display: flex;
  align-items: flex-end;
  text-decoration: none;
  border: 4px solid #b0215e;
  margin-bottom: 20px;
  background-image: url('../assets/Screenshot_18.png'); 
    background-size: cover;
  
  @include media {
    height: 500px;
  }
}

.inner {
  height: 50%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center; 
  background: white;
  box-sizing: border-box;
  padding: 40px;
  
  @include media {
    width: 50%;
    height: 100%;
  }
}

.title {
  font-size: 24px;
  color: black;  
  text-align: center;
  font-weight: 700;
  color: #181818;
  text-shadow: 0px 2px 2px #a6f8d5;
  position: relative;
  margin: 0 0 20px 0;
  
  @include media {
    font-size: 30px;
  }
}

.subtitle {
  color: #b0215e;
  text-align: center;
}


</style>