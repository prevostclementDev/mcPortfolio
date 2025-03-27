<script setup lang="ts">

</script>

<template>
  <div>
    <div class="about">

      <div class="text">
        <h1>Un peu sur moi...</h1>
        <p>
          Maurine, 21 ans, je viens de terminer ma licence en Web-design à Mydigitalschool.
          <br><br>
          Passionnée par l’image et la création, je profite de cette année pour plonger dans l'entrepreneuriat en tant que Content Creator, avant d’entamer un Master en Direction Artistique.
          <br><br>
          Toujours inspirée par mes expériences et mon environnement, j’aime capturer des instants authentiques et raconter des histoires visuelles qui vous plongent dans des moments uniques.
          <br><br>
          Chaque projet est une nouvelle exploration, une opportunité de me dépasser et de m’adapter, car chaque image raconte sa propre histoire.
          <br><br>
          Ma devise : « Une nouvelle aventure, une nouvelle image... »
          <br><br>
          Curieux de découvrir mon univers ? N’hésites pas à explorer mon travail et laisses-toi embarquer dans mon monde !
        </p>
      </div>

      <div class="img">
        <img src="/about.png" alt="">
      </div>

    </div>
    <img class="bandeau" src="/about2.png" alt="">
  </div>
</template>

<style scoped>
.about {
  display: flex;
  flex-direction: row;
  margin: 100px 0;
  position: relative;
  
  @media screen and (max-width: 857px) {
    flex-direction: column;
    align-items: center;
    margin: 50px 0;

  }

  .text {
    width: 70%;
    color: white;
    padding-left: 72px;

    @media screen and (max-width: 857px) {
      padding-left: 0;
      width: 70%;

    }

    @media screen and (max-width: 629px) {
      width: 90%;

    }

    h1 {
      font-size: 25px;
      font-weight: 700;
      @media screen and (max-width: 1017px) {
        font-size: 20px;
      }

    }

    p {
      font-weight: 400;
      font-size: 20px;
      margin-top: 50px;
      max-width: 70%;
      
      @media screen and (max-width: 1017px) {
        font-size: 16px;
      }

      @media screen and (max-width: 857px) {
        max-width: 100%;

      }

    }

  }

  .img {
    width: 30%;
    display: flex;
    justify-content: flex-end;

    @media screen and (max-width: 857px) {
      width: 100%;

    }
    @media screen and (max-width: 629px) {
      margin-top: 20px;

      img {
        width: 70%;
        object-fit: contain;

      }

    }

  }

  &::before {
    content: "";
    position: absolute;
    bottom: 0;
    right: 0;
    width: 70%;
    height: 2px;
    background: white;

  }

}
.bandeau {
  width: 100%;
  object-fit: cover;
  object-position: center;
  margin-bottom: 100px;

  @media screen and (max-width: 675px) {
    height: 200px;

  }

}
</style>