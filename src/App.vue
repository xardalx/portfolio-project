<template>
    <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <!--  -->
      <div id="menu">
      <br>
      <a href="#section1" style="color:black">ABOUT</a>
      <br>
      <a href="#section2" style="color:black">VIDEO CV</a>
      <br>
      <a href="#section3" style="color:black">PORTFOLIO</a>
      <br>
      <a href="#cvpic" style="color:black">RESUME</a>
      <br>
      <a href="#section5" style="color:black">CONTACT</a>
      </div>
    </v-navigation-drawer>

    <v-app-bar app>
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>

      <v-toolbar-title>ARDAL Portfolio</v-toolbar-title>
    </v-app-bar>
    

    <v-main>


      <!-- Content stuff -->
  
      <div id="section1">
        <h1>ABOUT ARDAL</h1>
        <div id="ABOUT ARDAL">
          <article>
            Visual media designer specialising in video production and photography. From a small <br>
            fishing town in Iceland, currently living in Esbjerg, Denmark for studying. Worked on <br>
            projects ranging from interviews and video production for Reykjavík-based production <br>
            company Ursus Parvus to freelance photography gigs for Icelandic ARENA swimwear <br>
            distributor and local supplement store Bætiefnabúllan.
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
        <h1>PORTFOLIO - Photography, Graphic design and Video</h1>
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
      </div>

      <div id="section32">
                <div class="gallery2">
          <a target="_blank" href="kari1.jpg">
          <img src="./assets/kari1.jpg" alt="KARI" width="600" height="400">
          </a>
        <div class="desc">KARI</div>
          </div>

        <div class="gallery2">
          <a target="_blank" href="kari2.jpg">
            <img src="./assets/kari2.jpg" alt="KARI2" width="600" height="400">
          </a>
          <div class="desc">KARI</div>
        </div>

        <div class="gallery2">
          <a target="_blank" href="kari3.jpg">
            <img src="./assets/kari3.jpg" alt="KARI3" width="600" height="400">
          </a>
          <div class="desc">KARI</div>
        </div>

        <div class="gallery2">
          <a target="_blank" href="kari4.jpg">
            <img src="./assets/kari4.jpg" alt="KARI4" width="600" height="400">
          </a>
          <div class="desc">KARI</div>
        </div>
      </div>

      <div id="section33">
        <div class="gallery2">
          <a target="_blank" href="2work.png">
          <img src="./assets/2work.png" alt="2WORK" width="600" height="400">
          </a>
        <div class="desc">2work</div>
          </div>

        <div class="gallery2">
          <a target="_blank" href="bull.png">
            <img src="./assets/bull.png" alt="BULL" width="600" height="400">
          </a>
          <div class="desc">BULL</div>
        </div>

        <div class="gallery2">
          <a target="_blank" href="idea.png">
            <img src="./assets/idea.png" alt="IDEA" width="600" height="400">
          </a>
          <div class="desc">IDEA HOUSE</div>
        </div>

        <div class="gallery2">
          <a target="_blank" href="soley.png">
            <img src="./assets/soley.png" alt="SOLEY" width="600" height="400">
          </a>
          <div class="desc">SOLEY</div>
        </div>
      </div>

      <div id="section35">
        <div id="shortfilm">
          <iframe width="560" height="315" src="https://www.youtube.com/embed/FmBXdCh3oWw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        </div>
      </div>

        <v-img id="cvpic"
        :src="require('./assets/cv.jpg')"></v-img>

      <div id="section45">
        <v-img id="bottombg"
        :src="require('./assets/bottombg.png')"></v-img>
      </div>

      <div id="section5">
        <div id="contact_info">
        <h1>CONTACT INFO</h1>
        <br>
        +45 24 80 26 56
        <br>
        <a href="mailto:olafur.sig99@outlook.com" style="color:white">olafur.sig99@outlook.com</a>
        <br>
        <a href="https://www.linkedin.com/in/xardalx/" style="color:white">LinkedIn</a>
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

  #h2 :hover {
    opacity: 70%;
  }

  #ardaltop {
    padding-left: 25%;
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
    height: 500px;
    padding-left: 25%;
    padding-top: 10%;
    margin: 0;
    padding-right: 5%;
    padding-bottom: 5%;
    
  }

  #section32 {
    height: 300px;
    justify-content: center;
    align-items: center;
    padding-top: 5%;
    padding-left: 25%;
  }

  #section33 {
    height: 500px;
    justify-content: center;
    align-items: center;
    padding-bottom: 10%;
    padding-left: 25%;
  }

  #section35 {
    justify-content: center;
    align-items: center;
    padding-left: 25%;
    padding-bottom: 10%;
  }

  #section4 {
    height: 2480px;
    justify-content: center;
    align-content: center;
    background-color: white;
    padding: 0;
  }

  #section45 {
    padding: 0;
  }

  #contact_info {
    background-color: black;
    font-family: Arial, Helvetica, sans-serif;
    color: white;
    padding-bottom: 50px;
    padding-top: 50px;
    padding-left: 50px;
    font-size: 16pt;
  }

  menu {
    font-family: Arial, Helvetica, sans-serif;
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

div.gallery2 {
  margin: 5px;
  border: 1px solid #ccc;
  float: left;
  width: 180px;
}

div.gallery2:hover {
  border: 1px solid #777;
}

div.gallery2 img {
  width: 100%;
  height: auto;
}

a {
  text-decoration: none;
  color: black;
  font-size: 24pt;

}

a:hover {
  opacity: 70%;
 }

 spacer {
   height: 200px;
 }

</style>