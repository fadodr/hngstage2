<template>
<div class="appcontainer">
  <img class="hngimg" src="./assets/HNG.png" alt="" height="100" width="200">
  <div class="header">
      <h3>My Resume</h3>
      <div class="underline"></div>
  </div>
  <div class="app-container">
    <app-left class="left-container"></app-left>
    <app-right class="right-container"></app-right>
  </div>
  <app-footer></app-footer>
</div>
</template>

<script>
import leftcomponent from '@/components/leftcomponent'
import rightcomponent from '@/components/rightcomponent'
import footer from '@/components/footer'
export default {
  components: {
    appLeft : leftcomponent,
    appRight : rightcomponent,
    appFooter : footer
  }
}
</script>

<style>
.app-container {
  width: 100%;
}
.header {
  display: flex;
  justify-content: center;
  flex-direction: column;
  color: #707070;
  height: 70px;
  align-items: center;
}
.hngimg {
  margin: auto;
  display: block;
  padding: 15px 0;
}
h3 {
  font-family: "jost";
  font-size: 35px;
  margin: 0;
  width: max-content;
}
.underline {
  height: 5px;
  width: 100px;
  display: flex;
  justify-content: center;
  background-color: #f9b247;
}
  .app-container {
    display: flex;
  }
  .left-container {
  width: 30%;}
  .right-container {
  width: 70%;}
  @media screen and (max-width: 970px) {
    .app-container {
    flex-direction: column;}
    .left-container {
  width: 100%;}
  .right-container {
  width: 100%;}
  }
</style>