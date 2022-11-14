<script setup>
import headerVue from './components/header.vue';
import aboutVue from './components/about.vue';
import contactVue from './components/contact.vue';

</script>

<template>
  <div class="container">
    <headerVue nama="Fadilatur Rohman"/>

    <aboutVue/>

    <contactVue/>
  </div>
</template>

<style >
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Courier New', Courier, monospace;
}
body{
  padding: 4.5rem;
  background-color: rgb(101, 101, 101);
}
.container{
  background-color: rgb(235, 234, 234);
  
}
.header{
  background-color: rgb(10, 116, 229);
  display: flex;
  align-items: center;
  column-gap: 8rem;
  padding: 4rem 5rem;
}
.header__container{
  display: flex;
  flex-direction: column;
  row-gap: 1rem;
  color: #fff;
}
.header img{
  transform: translateY(80px);
  border: 5px solid #fff;
}
.header__container h1{
  font-size: 2.5rem;
}
.header__container h3{
  font-size: 1.5rem;
}
.header__btn button{
  border: 0;
  padding: .8rem 1rem;
  font-weight: bold;
  font-size: 1rem;
  border-radius: 2rem;
}
.header__btn button:nth-child(2){
  background-color: rgb(4, 114, 15);
  color: #fff;
  margin-left: .5rem;
}

/* ================ */
.about{
  padding: 3.5rem 4rem;
}
.about__container{
  display: flex;
  column-gap: 4rem;
  margin-top: 2rem;
}
.col__about:nth-child(1){
  line-height: 1.8;
  flex-basis: 50%;
}
.col__about{
  display: grid;
  row-gap: 1rem;
}
/* ========= */
.contact{
  padding: 3.5rem 4rem;
}
.contact__container{
  display: flex;
  column-gap: 4rem;
  margin-top: 2rem;
}
.col__contact{
  width: 50%;
}
.col__contact:nth-child(2){
  display: flex;
  flex-direction: column;
  row-gap: 1rem;
}
.contact__input input{
  padding: .5rem;
  width: 252px;
  margin-bottom: .5rem;
}
textarea{
  padding: .5rem;
}
.btn__kirim {
  display: block;
  padding: .5rem .7rem;
  border-radius: 2rem;
  background-color: rgb(36, 36, 233);
  color: #fff;
  border: none;
  margin-top: 1rem;
  cursor: pointer;
}
@media only screen and (max-width: 576px){
  body{
      padding: 0;
  }
  .header{
      flex-wrap: wrap;
      padding: 3rem 2rem;
      text-align: center;
      justify-content: center;
  }
  .header img{
      transform: translateY(0);
      margin-bottom: 2rem;
  }
  .header__container h1{
      font-size: 2rem;
  }
  .header__container h3{
      font-size: 1rem;
      margin-bottom: 2rem;
  }
  .header__container{
      row-gap: .5rem;
  }
  /* =================== */
  .about{
      padding: 3rem 1.5rem;
  }
  .about__container{
      display: flex;
      flex-wrap: wrap;
      column-gap: 1.1rem;
      row-gap: 1.8rem;
  }
  .col__about:nth-child(1){
      /* line-height: 1.8; */
      flex-basis: 100%;
  }
  /* =================== */
  .contact{
      padding: 3rem 1.5rem;
  }
  .contact__container{
      flex-wrap: wrap;
      column-gap: 0;
      row-gap: 2rem;
      margin-top: 0;
  }
  .contact__input input{
      width: 100%;
  }
  textarea{
      width: 100%;
  }
  
}
</style>

