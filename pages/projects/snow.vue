<script setup lang="ts">
</script>

<template>
  <project-page-title
      title="SHOOTING SNOWBOARD"
      text1=""
      text2="Edit : MC Production"
  />

  <div class="galerie">

    <div class="element">
      <img src="~/public/projects/snow/1.png" alt="" />
    </div>

    <div class="element">
      <img src="~/public/projects/snow/2.png" alt="" />
    </div>

    <div class="element">
      <img src="~/public/projects/snow/3.png" alt="" />
    </div>

    <div class="element">
      <img src="~/public/projects/snow/4.png" alt="" />
    </div>

    <div class="element">
      <img src="~/public/projects/snow/5.png" alt="" />
    </div>

    <div class="element">
      <img src="~/public/projects/snow/6.png" alt="" />
    </div>

  </div>

</template>

<style scoped>
.galerie {
  padding: 45px;
  display: flex;
  justify-content: flex-start;
  align-items: stretch;
  flex-wrap: wrap;
  gap: 30px;

  .element {
    width: calc(100% / 3 - 30px);

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;

    }

  }

}
</style>