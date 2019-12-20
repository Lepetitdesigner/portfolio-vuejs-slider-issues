<template>
  <div>
    <header>
      <div class="d-flex">
        <div class="logo">
          <img src="./img/logo.png">
        </div>
        <nav>
          <ul>
            <li><a href="#">Présentation</a></li>
            <li><a href="#">Projet</a></li>
            <li><a href="#">CV</a></li>
          </ul>
        </nav>
      </div>
    </header>
    <carousel>
    <carousel-slide>
      <div class="bg">
        <img src="./img/first-bg.svg" alt="">
      </div>
      <div class="size1 d-flex2">
        <div>
          <img src="./img/profil.png">
        </div>
        <div>
          <h2>Bonjour et bienvenue sur mon portfolio</h2>
          <div class="l-h">
            <p>Quentin Rulleau,  22 ans. Habitant en Picardie et développeur Front-End junior.</p>
            <br>
            <p>Fan de la culture geek, je suis intéréssé par tout ce qui m'entoure et je suis <br>curieux de la vie.</p>
          </div>
          <p class="ajust">“La simplicité est la sophistication suprême.” Léonard de Vinci</p>
          <div class="ajust1">
            <a href="#">MES PROJETS</a>
            <a href="#">AUCUNE IDEE</a>
          </div>
        </div>
      </div>
    </carousel-slide>

      <carousel-slide>
        <div class="bg1">
          <img class="h-100" src="./img/second-bg.svg" alt="">
        </div>
         <h3 class="t-center ajust4">VOULEZ-VOUS vous <span>mettre en avant sur le monde numérique ?</span></h3>
         <div class="size3 d-flex2">
          <div class="">
            <img src="./img/skill.svg" alt="">
          </div>
          <div>
            <h4>Je mets à disposition mes compétences pour répondre au mieux à vos besoins</h4>
            <div class="d-flex2">
              <div class="">
                <div class="d-flex3 ml">
                  <img src="./img/line.svg" alt="">
                  <p>Création d’un sitre vitrine / ecommerce</p>
                </div>
                <div class="d-flex3 espace">
                  <img src="./img/line.svg" alt="">
                  <p>Création d’une identité numérique</p>
                </div>
                <div class="d-flex3">
                  <img src="./img/line.svg" alt="">
                  <p>Création de solution graphique</p>
                </div>
              </div>
              <div class="">
                <div class="d-flex3">
                  <img src="./img/line.svg" alt="">
                  <p>référencement naturel</p>
                </div>
                <div class="d-flex3 espace">
                  <img src="./img/line.svg" alt="">
                  <p>Mise en place d’un emailing efficace</p>
                </div>
                <div class="d-flex3">
                  <img src="./img/line.svg" alt="">
                  <p>Design responsive</p>
                </div>
              </div>
            </div>
          </div> 
         </div>
      </carousel-slide>

      <carousel-slide>
        <div class="bg1">
          <img src="./img/third-bg.svg" alt="">
        </div>
        <div class="size2 d-flex2">
          <div>
            <img src="./img/film.jpg" alt="">
            <img src="./img/hobbies-esport-quentin-rulleau-webdesigner-lepetitdesigner.jpg" alt="">
            <img src="./img/technologie.png" alt="">
          </div>
          <div class="ajust2">
            <h2>Mes hobbies</h2>
            <p class="ajust3">Je suis un amateur de film inspiré d’histoire vraie , en paticulier remember the titans  qui est réalisé par Boaz Yakin et produit par Jerry Bruckheimerest. C’est ce film qui m’a le plus marqué par ses valeurs.</p>
            <p>De même je suis un grand fan d’esport , j’aime l’esprit de compétition qui s’en dégage. Ce qui m’a amené à m’intéresser à la technologie et ses innovations.</p>
          </div>
        </div>
      </carousel-slide>

      <carousel-slide>
        <div class="bg1">
          <img class="h-100" src="./img/fourth-bg.svg" alt="">
        </div>
        <h3 class="t-center fourth">Pour répondre au mieux à votre demande, je travaille avec ces outils</h3>
        <div class="d-flex2 size4">
          <div class="d-flex2">
            <div>
              <h4>Langage de Code</h4>
              <p>HTML & CSS</p>
              <p>Javascript</p>
              <p>PHP</p>
            </div>
            <div class="espace1">
              <h4>Logiciel</h4>
              <p>Figma</p>
              <p>Adobe photoshop 2019 CC</p>
              <p>Adobe Indesign 2019 CC</p>
              <p>Adobe  illustrator 2019 CC</p>
            </div>
          </div>
          <img src="./img/tools.svg" alt="">
        </div>
      </carousel-slide>

    </carousel>
  </div>
</template>

<script>

  import Carousel from './components/carousel/carousel'

  import CarouselSlide from './components/carousel/carouselSlide'

  export default {
    data () {
      return {

      }
    },
    methods: {

    },
    components: {
      Carousel,
      CarouselSlide
    }
  }
</script>

<style src="./styles/styles.css"></style>
