<template>
    <section class="counters">
      <div class="container">
        <div>
          <i class="fab fa-youtube fa-4x"></i>
          <div class="counter" data-target="9000"><vue3-autocounter ref='counter' :startAmount='0' :endAmount='2021' :duration='10' /></div>
          <h4>Subscribers</h4>
        </div>
        <div>
          <i class="fab fa-twitter fa-4x"></i>
          <div class="counter" data-target="15000"><vue3-autocounter ref='counter' :startAmount='0' :endAmount='1300' :duration='10' /></div>
          <h4>Followers</h4>
        </div>
        <div>
          <i class="fab fa-facebook fa-4x"></i>
          <div class="counter" data-target="9000"><vue3-autocounter ref='counter' :startAmount='0' :endAmount='700' :duration='10' /></div>
          <h2>Likes</h2>
        </div>
        <div>
          <i class="fab fa-linkedin fa-4x"></i>
          <div class="counter" data-target="5000"><vue3-autocounter ref='counter' :startAmount='0' :endAmount='1800' :duration='10'  /></div>
          <h5>Connections</h5>
        </div>
      </div>
    </section>
    </template>

    <script>
      import { defineComponent } from 'vue';
      import Vue3autocounter from 'vue3-autocounter';

       export default defineComponent({
       name: 'AnimCount',
       components: {
       'vue3-autocounter': Vue3autocounter
       },
       PROPS: {
       duration: {
       type: Number,
       default: 3,
       validate: (duration) => {
        return duration >= 1;
       }
       },
       }
      });
    
      
    
    


    </script>

    <style scoped>

    

  * {
   box-sizing: border-box;
    margin: 0;
     padding: 0;
  }

  body {
  font-family: 'Roboto', sans-serif;
  background: lightskyblue
    url('https://i.pinimg.com/originals/3c/24/46/3c24462450c2a902bf7e18f3d9aada81.jpg');
  color: #fff;
  /* Push to bottom */
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  height: 100vh;
}

.container {
  max-width: 1100px;
  margin: 0 auto;
  overflow: auto;
}

header {
  flex: 1;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

header h1 {
  font-size: 60px;
}

.counters {
  background: #4F46E5;
  color: #fff;
  padding: 40px 20px;
  border-top: 3px lightskyblue solid;
}

.counters .container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-gap: 30px;
  text-align: center;
}

.counters i {
  color: lightskyblue;
  margin-bottom: 5px;
}

.counters .counter {
  font-size: 45px;
  margin: 10px 0;
}

   @media (max-width: 700px) {
  .counters .container {
    grid-template-columns: repeat(2, 1fr);
  }

  .counters .container > div:nth-of-type(1),
  .counters .container > div:nth-of-type(2) {
    border-bottom: 1px lightskyblue solid;
    padding-bottom: 20px;
  }
}

    </style>