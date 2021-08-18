<template>
  <div>
    <div class="circle" :class="{ changecircle: remove }"></div>
    <div class="resume-container">
      <div class="line"></div>
      <div>
        <div class="box" v-for="i in infos" :key="i.title">
          <div class="date-header">
            <p>{{ i.date }}</p>
          </div>
          <div class="personal-info">
            <p class="personal-header">{{ i.title }}</p>
            <p class="personal-title">Fado Inc.</p>
            <p class="personal-body">
              {{ i.body }}
            </p>
          </div>
        </div>
        <div v-vpshow class="skills-container">
          <p>- CODING SKILLS -</p>
        </div>
        <div v-vpshow class="skills">
          <p class="language">FLUTTER</p>
          <div class="progress-container">
            <div class="progress"></div>
            <p>90%</p>
          </div>
          <p class="language">VUEJS</p>
          <div class="progress-container">
            <div class="progress2"></div>
            <p>85%</p>
          </div>
          <p class="language">NODE JS</p>
          <div class="progress-container">
            <div class="progress3"></div>
            <p>90%</p>
          </div>
          <p class="language">HTML, CSS & JAVASCRIPT</p>
          <div class="progress-container">
            <div class="progress4"></div>
            <p>80%</p>
          </div>
        </div>
      </div>
    </div>
    <button>DOWNLOAD CV</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      infos: [
        {
          date: "DEC 2018 -  JAN 2020",
          title: "FRONTEND DEVELOPER",
          body: `I acquired my HTML, CSS, JAVASCRIPT knowledge from Udemy and with the help of youtube and online resource
          i was able to complete my learning and be profecient with the technologies`,
        },
        {
          date: "MAR 2020 - JUNE 2020",
          title: "BACKEND DEVELOPER",
          body: `I gained my backend and database management knowledge from Udemy and also from youtube and online resource. i learnt Nodejs both the
          expressjs and grapql framework and i was able to build a server-side code and also with the ability to work with mongoDB`,
        },
        {
          date: "JUNE 2020 - SEPT 2020",
          title: "MOBILE APP DEVELOPER",
          body: `I gained my mobile app knowledge from Udemy as well and i was able to build a cross platform appluication that work
          for both andrioid and ios`,
        },
        {
          date: "SEPT 2020 - CURRENNT",
          title: "FULLSTACK DEVELOPER",
          body: `I currently work with vuejs, expressjs, mongoDB and flutter and still learning other new technologies such as nuxtjs too`,
        },
      ],
    };
  }
}
</script>

<style scoped>
.resume-container {
  width: 100%;
  display: flex;
  justify-content: space-between;
}
.line {
  width: 3px;
  margin-right: 50px;
  background-color: #b7b7b7;
  border: 1px solid #b7b7b7;
}
.date-header {
  width: max-content;
  padding: 0 15px;
  border: 2px solid #f9b247;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 15px 0;
  margin-top: 30px;
}
.date-header p {
  font-family: "jost";
  font-size: 14px;
  color: #f9b247;
}
.personal-info {
  margin-left: 40px;
}
.personal-header {
  font-family: "jost";
  font-size: 18px;
  font-weight: 600;
}
.personal-title {
  font-family: "jost";
  font-size: 16px;
  color: #b7b7b7;
}
.personal-body {
  font-family: "jost";
  font-size: 18px;
  color: #707070;
}
p {
  margin: 7px 0;
}
.circle {
  width: 15px;
  height: 15px;
  border-radius: 50%;
  background-color: #f9b247;
  margin-left: -5px;
}
.skills-container {
  width: 100%;
  height: 70px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.skills-container p {
  font-family: "jost";
  font-size: 20px;
  font-weight: 600;
}
.skills {
  width: 80%;
  margin: 0 auto;
  margin-bottom: 50px;
}
.progress-container {
  width: 80%;
  height: 7px;
  background-color: #b7b7b7;
  margin-bottom: 20px;
  border-radius: 4px;
  display: flex;
  flex-direction: row;
  overflow: visible;
}
.progress {
  width: calc(90% - 41px);
  height: 7px;
  border-radius: 4px;
  background-color: #f9b247;
}
.progress2 {
  width: calc(85% - 41px);
  height: 7px;
  border-radius: 4px;
  background-color: #f9b247;
}
.progress3 {
  width: calc(90% - 41px);
  height: 7px;
  border-radius: 4px;
  background-color: #f9b247;
}
.progress4 {
  width: calc(80% - 41px);
  height: 7px;
  border-radius: 4px;
  background-color: #f9b247;
}
button {
  color: #f9b247;
  border: 2px solid #f9b247;
  background-color: white;
  padding: 15px 20px;
  font-family: "jost";
  font-size: 16px;
  cursor: pointer;
  font-weight: bold;
  border-radius: 5px;
  margin-left: -7px;
  margin-bottom: 15px;
}
.progress-container p {
  width: max-content;
  padding: 15px 3px;
  border: 1px solid black;
  font-family: "jost";
  background-color: white;
  color: #707070;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 18px;
  font-weight: 500;
  overflow: visible;
  margin-top: -10px;
}
.language {
  font-family: "jost";
  font-size: 14px;
  font-weight: 600;
}
@media screen and (max-width: 970px) {
    .circle {
  width: 15px;
  height: 15px;
  border-radius: 50%;
  background-color: #f9b247;
  position: initial;
    margin: 0;
  }
  .line {
  margin-left: 5px;
}
}
</style>
