<template>
  

  <div class="window">
  
  
  <h1>Bilgiler</h1>
  <h4>İsim: {{ isim }}</h4>
  <h4>Soyisim: {{ soyisim }}</h4>
  <h4>Yaş: {{ yas }}</h4>
  <h4>Bölüm: {{ bölüm }}</h4>
  <h4>Proje sayısı: {{ sayi }}</h4>
  
  
  <div class="d-flex gap-2">
  
  <button @click="arttir" class="btn btn-success">Arttır</button>
  <button @click="azalt"  class="btn btn-danger ">Azalt</button>
  
  </div>
  
  
  </div>
  
  </template>
  
  
  
  
  
  
  <script>
  
  
  export default {
    name: 'App',
  
    data() {
      return {
        
        isim: "Gülseren",
        soyisim: "Zamir",
        yas: 21,
        bölüm: "Bilgisayar Mühendisliği",
        sayi:0
      }
    },
  
    methods:{
  
      arttir(){
        this.sayi++;
      },
      azalt(){
        
       this.sayi--;
  
      }
  
    },
  
    mounted() {
      
      
    },
   
  }
  </script>
  
  
  
  
  
  
  
  
  <style>
  
  .window{
    width:100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin-top: 3rem ;
  }
  
  
  
  </style>
  