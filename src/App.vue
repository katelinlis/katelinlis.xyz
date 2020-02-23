<template>
  <div id="app">    
    <div class="card">
      <div class="card-body" style="height: 248px">
        <div>
          <div  class=" d-flex flex-column flex-md-row align-items-center p-3 px-md-4 mb-3 bg-white" v-bind:class="{'fixed-top border-bottom shadow-sm':StickyHeader}">
            <h5 class="my-0 mr-md-auto font-weight-normal">Katelinlis</h5>
            <nav class="my-2 my-md-0 mr-md-3">
              <a class="p-2 text-dark" href="#about">About</a>
              <a class="p-2 text-dark" href="#tech">Tech</a>
              <a class="p-2 text-dark" href="#social">Social</a>
            </nav>
          </div>
            <p style="padding-left: 1.5rem !important; text-align:center;" class="lead font-italic  my-3">Привет! Меня зовут Кейтлин. <br>
              Я работаю в сфере веб разработки 5 лет <br>
              Я могу для вас разработать клиентскую или серверную часть для вашего сайта<br>
              А так же помочь в доработке той или иной идеи
            </p>
          </div>
        </div>
      </div>
    <contentPage/>
  </div>
</template>

<script>


import contentPage from '@/components/content'

export default {
  data(){
    return {
      StickyHeader: false
    }
  },
  created() {
    
    window.addEventListener('scroll', ()=> {
      console.log( pageYOffset);
      if(pageYOffset >= 280) this.StickyHeader = true
      else this.StickyHeader = false
    });
  },
  components: {

    contentPage
  },
  name: 'App',
}
</script>

<style>

  .container {
    padding-top: 30px;
  }
  .mainCard{
    background: rgba(237,237,237,1);
    background: -moz-linear-gradient(45deg, rgba(237,237,237,1) 0%, rgba(246,246,246,1) 47%, rgba(237,237,237,1) 100%);
    background: -webkit-gradient(left bottom, right top, color-stop(0%, rgba(237,237,237,1)), color-stop(47%, rgba(246,246,246,1)), color-stop(100%, rgba(237,237,237,1)));
    background: -webkit-linear-gradient(45deg, rgba(237,237,237,1) 0%, rgba(246,246,246,1) 47%, rgba(237,237,237,1) 100%);
    background: -o-linear-gradient(45deg, rgba(237,237,237,1) 0%, rgba(246,246,246,1) 47%, rgba(237,237,237,1) 100%);
    background: -ms-linear-gradient(45deg, rgba(237,237,237,1) 0%, rgba(246,246,246,1) 47%, rgba(237,237,237,1) 100%);
    background: linear-gradient(45deg, rgba(237,237,237,1) 0%, rgba(246,246,246,1) 47%, rgba(237,237,237,1) 100%);
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#ededed', endColorstr='#ededed', GradientType=1 );
  }

  .MyTechs{
    margin-bottom: 30px;
    background: rgba(242,234,242,1);
    background: -moz-linear-gradient(45deg, rgba(242,234,242,1) 0%, rgba(255,232,255,1) 100%);
    background: -webkit-gradient(left bottom, right top, color-stop(0%, rgba(242,234,242,1)), color-stop(100%, rgba(255,232,255,1)));
    background: -webkit-linear-gradient(45deg, rgba(242,234,242,1) 0%, rgba(255,232,255,1) 100%);
    background: -o-linear-gradient(45deg, rgba(242,234,242,1) 0%, rgba(255,232,255,1) 100%);
    background: -ms-linear-gradient(45deg, rgba(242,234,242,1) 0%, rgba(255,232,255,1) 100%);
    background: linear-gradient(45deg, rgba(242,234,242,1) 0%, rgba(255,232,255,1) 100%);
    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#f2eaf2', endColorstr='#ffe8ff', GradientType=1 );
  }
</style>
