<template>
    <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <!--  -->
      <div id="menu">
      <a href="#section1">ABOUT</a>
      <br>
      <a href="#section2">VIDEO CV</a>
      <br>
      <a href="#section3">PORTFOLIO</a>
      <br>
      <a href="#section4">RESUME</a>
      <br>
      <a href="#section5">CONTACT</a>
      </div>
    </v-navigation-drawer>

    <v-app-bar app>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>ARDAL</v-toolbar-title>
    </v-app-bar>
    

    <v-main>


      <!-- Content stuff -->
    
      <div id="section1">
        <h1>ABOUT ARDAL</h1>
        <div id="ABOUT ARDAL">
          <article>
            Visual media designer specialising in video production and photography.
          </article>
        </div>
      </div>
    
      <div id="section2">
        <div id="VIDEO CV">
          <section>
            <iframe width="560" height="315" src="https://www.youtube.com/embed/pgRlRicH4KE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
          </section>
        </div>
      </div>

      <div id="section3">
        <h1>PORTFOLIO</h1>
        <br>

        <div class="gallery">
          <a target="_blank" href="IMG_3516.jpg">
          <img src="./assets/IMG_3516.jpg" alt="ARENA" width="600" height="400">
          </a>
        <div class="desc">ARENA Project</div>
          </div>

        <div class="gallery">
          <a target="_blank" href="IMG_3626.jpg">
            <img src="./assets/IMG_3626.jpg" alt="ARENA2" width="600" height="400">
          </a>
          <div class="desc">ARENA Project</div>
        </div>

        <div class="gallery">
          <a target="_blank" href="IMG_3571.jpg">
            <img src="./assets/IMG_3571.jpg" alt="ARENA3" width="600" height="400">
          </a>
          <div class="desc">ARENA Project</div>
        </div>

        <div class="gallery">
          <a target="_blank" href="kat.jpg">
            <img src="./assets/kat.jpg" alt="ARENA4" width="600" height="400">
          </a>
          <div class="desc">ARENA Project</div>
        </div>

        <div class="gallery">
          <a target="_blank" href="kari1.jpg">
          <img src="./assets/kari1.jpg" alt="KARI" width="600" height="400">
          </a>
        <div class="desc">KARI</div>
          </div>

        <div class="gallery">
          <a target="_blank" href="kari2.jpg">
            <img src="./assets/kari2.jpg" alt="KARI2" width="600" height="400">
          </a>
          <div class="desc">KARI</div>
        </div>

        <div class="gallery">
          <a target="_blank" href="kari3.jpg">
            <img src="./assets/kari3.jpg" alt="KARI3" width="600" height="400">
          </a>
          <div class="desc">KARI</div>
        </div>

        <div class="gallery">
          <a target="_blank" href="kari4.jpg">
            <img src="./assets/kari4.jpg" alt="KARI4" width="600" height="400">
          </a>
          <div class="desc">KARI</div>
        </div>

        <div id="shortfilm">
          <iframe width="560" height="315" src="https://www.youtube.com/embed/FmBXdCh3oWw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        </div>
     
        
      </div>

      <div id="section4">
        <v-img id="cvpic"
        :src="require('./assets/cv.jpg')"></v-img>
      </div>

      <div id="section45">
        <v-img id="bottombg"
        :src="require('./assets/bottombg.png')"></v-img>
      </div>

      <div id="section5">
        <div id="contact_info">
        <h1>CONTACT INFO</h1>
        <br>
        <h2>+45 24 80 26 56</h2>
        <a href="mailto:olafur.sig99@outlook.com"><h2>olafur.sig99@outlook.com</h2></a>
        <a href="https://www.linkedin.com/in/xardalx/"><h2>LinkedIn</h2></a>
        </div>
      </div>
    
    </v-main>
  </v-app>
</template>

<script>


export default {
  name: 'App',

  components: {
 
  },

 data: () => ({ 
   drawer: false 
  }),
};
</script>


<style lang="scss">
  #h1 {
    font-family: Arial, Helvetica, sans-serif;
    color: black;
  }
  
  #section1 {
    height: 500px;
    padding-top: 10%;
    padding-left: 25%;
  }

  #section2 {
    height: 500px;
    padding-left: 25%;
    justify-content: center;
  }

  #section3 {
    height: 1000px;
    padding-left: 25%;
    padding-top: 10%;
    margin: 0;
    padding-right: 5%;
    
  }

  #section4 {
    height: 2480px;
    justify-content: center;
    align-content: center;
    background-color: white;
  }

  #section45 {
    padding: 0;
  }

  #contact_info {
    background-color: black;
    font-family: helvetica, sans-serif;
    color: white;
    padding-bottom: 50px;
    padding-top: 50px;
    padding-left: 50px;
  }

  #menu {
    font-family: helvetica;
    color: white;
    padding: 8px 16px;

  }

  div.gallery {
  margin: 5px;
  border: 1px solid #ccc;
  float: left;
  width: 180px;
}

div.gallery:hover {
  border: 1px solid #777;
}

div.gallery img {
  width: 100%;
  height: auto;
}

div.desc {
  padding: 15px;
  text-align: center;
}
</style>