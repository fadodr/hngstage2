<template>
    <div class="row footer">
        <p class="devfado">Dev Fado</p>
        <div class="footerimg">
           <div class="minicircle"><img src="~@/assets/facebook2.svg"  alt="" height="20" width="20"></div>
           <div class="minicircle"><img src="~@/assets/whatsapp2.svg" alt="" height="20" width="20"></div>
           <div class="minicircle"><img src="~@/assets/instagram2.svg" alt="" height="20" width="20"></div>
           <div class="minicircle"><img src="~@/assets/twitter2.svg" alt="" height="20" width="20"></div>
           <div class="minicircle"><img src="~@/assets/linkin2.svg" alt="" height="20" width="20"></div>
        </div>
            <p class="copyright">Copyright <span>Dev Fado</span>. All Rights Reserved.</p>
    </div>
</template>

<style scoped>
    .copyright span{
  font-weight: bold;
}
.devfado{
  font-family: 'jost';
  font-size: 30px;
  font-weight: bold;
  color: #707070;
}
.footer{
  padding: 30px 0;
  text-align: center;
  background-color: #F3F3F3;
}
    .footerimg{
      display: flex;
      justify-content: center;
      margin: 8px 0;
    }
    .footerimg{
      display: flex;
      justify-content: center;
      margin: 8px 0;
    }
    .minicircle {
      height: 40px;
      width: 40px;
      border-radius: 30px;
      margin: 0 7px;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: #F9B247;
    }
</style>