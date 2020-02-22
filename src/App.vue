<template>
  <div id="app">
    <FooterComponent/>
    <contentPage/>
  </div>
</template>

<script>

import FooterComponent from '@/components/FooterComponent'
import contentPage from '@/components/content'

export default {
  components: {
    FooterComponent,
    contentPage
  },
  name: 'App',
}
</script>

<style>

  .container {
    padding-top: 65px;
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
