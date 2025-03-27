<script setup lang="ts">

</script>

<template>
  <div id="home-header">
    <img id="home-header-img" src="~/public/home.png">
    <div id="home-header-content">
      <h1>Maurine Callot <br> <span>Une nouvelle <span class="b">aventure</span>, une nouvelle <span class="b">image...</span></span> </h1>
    </div>
  </div>
  <div id="home-content">

    <div id="home-realisation">
      <div class="line-text left">
        <p>Une <span>sélection</span> de mes <span>réalisations photos...</span></p>
        <div class="lines"></div>
      </div>

      <div id="realisation">
        <nuxt-link to="/projects/snow">
          <div class="imgSquare">
            <img src="~/public/projectsList/snow.png" alt="">
            <img src="~/public/projectsList/snowLight.png" alt="">
          </div>
        </nuxt-link>

        <nuxt-link to="/projects/baouw">
          <div class="imgSquare">
            <img src="~/public/projectsList/baouw.png" alt="">
            <img src="~/public/projectsList/baouwLight.png" alt="">
          </div>
        </nuxt-link>

        <nuxt-link to="/projects/dolomites">
          <div class="imgSquare">
            <img src="~/public/projectsList/dolo.png" alt="">
            <img src="~/public/projectsList/doloLight.png" alt="">
          </div>
        </nuxt-link>

<!--        <nuxt-link to="/projects/">-->
<!--          <div class="imgSquare">-->
<!--            <img src="~/public/projectsList/atlas.png" alt="">-->
<!--            <img src="~/public/projectsList/atlasLight.png" alt="">-->
<!--          </div>-->
<!--        </nuxt-link>-->

        <nuxt-link to="/projects/merlet">
          <div class="imgSquare">
            <img src="~/public/projectsList/merlet.png" alt="">
            <img src="~/public/projectsList/merletLight.png" alt="">
          </div>
        </nuxt-link>

        <nuxt-link to="/projects/perenecuisine">
          <div class="imgSquare">
            <img src="~/public/projectsList/peren.png" alt="">
            <img src="~/public/projectsList/perenLight.png" alt="">
          </div>
        </nuxt-link>

<!--        <nuxt-link to="/projects/serafino">-->
<!--          <div class="imgSquare">-->
<!--            <img src="~/public/projectsList/sera.png" alt="">-->
<!--            <img src="~/public/projectsList/seraLight.png" alt="">-->
<!--          </div>-->
<!--        </nuxt-link>-->
      </div>

      <div class="line-text right">
        <p>Contactez-moi pour mes réalisations vidéos... </p>
        <div class="lines"></div>
      </div>
    </div>

  </div>
</template>

<style scoped>
#home-header {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 0;

  #home-header-img {
    width: 100vw;
    height: 100vh;
    object-fit: cover;
    object-position: center;
    z-index: 0;
    position: relative;
    user-select: none;

  }

  #home-header-content {
    position: absolute;
    bottom: 10%;
    left: 5%;
    z-index: 1;
    color: white;

    h1 {
      font-size: 50px;
      font-weight: 900;
      line-height: 80%;

      span {
        font-size: 25px;
        font-weight: 400;

        &.b {
          font-weight: 800;

        }

      }

    }

  }

}
#home-content {
  margin-top: 100vh;
  color: white;
  font-size: 25px;

  .line-text {
    padding: 24px 48px;
    position: relative;
    margin: 12px 0;

    .lines {

      width: 70%;
      height: 2px;
      background: white;
      position: absolute;

    }

    &.right {
      text-align: right;

      .lines {
        right: 0;
        top: 0;

      }

    }

    &.left {

      .lines {
        left: 0;
        bottom: 0;

      }

    }

  }

  #realisation {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 2px;
    margin: 60px 0;

    a {
      display: contents;
    }

    .imgSquare {
      width: calc(100% / 3 - 2px);
      height: 325px;
      position: relative;

      @media screen and (max-width: 1360px) {
        height: 300px;
      }
      @media screen and (max-width: 1284px) {
        height: 275px;
      }
      @media screen and (max-width: 1210px) {
        width: calc(100% / 2 - 2px);
      }
      @media screen and (max-width: 802px) {
        height: 225px;
      }
      @media screen and (max-width: 665px) {
        height: 200px;
      }
      @media screen and (max-width: 577px) {
        width: 100%;
      }

      img {
        width: 100%;
        height: 100%;
        position: absolute;
        object-position: center;
        object-fit: cover;
        top: 0;
        left: 0;

        &:nth-child(1) {
          z-index: 0;
        }

        &:nth-child(2) {
          z-index: 1;
          opacity: 0;
          transition: .35s ease-in-out all;
          @media (hover: none) {
            opacity: 1;
          }
        }

      }

      &:hover {

        img {
          &:nth-child(2) {
            opacity: 1;

          }

        }

      }

    }

  }

}
</style>