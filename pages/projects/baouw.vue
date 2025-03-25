<script setup lang="ts">
</script>

<template>
  <project-page-title
      title="BAOUW ORGANIC NUTRITION"
      text1="Ancienne alternante web-designer graphiste"
      text2="Edit : MC Production"
  />

  <div class="galerie">

    <div class="element">
      <img src="~/public/projects/baouw/1.png" alt="" />
    </div>

    <div class="element">
      <img src="~/public/projects/baouw/2.png" alt="" />
    </div>

    <div class="element">
      <img src="~/public/projects/baouw/3.png" alt="" />
    </div>

    <div class="element">
      <img src="~/public/projects/baouw/4.png" alt="" />
    </div>

    <div class="element">
      <img src="~/public/projects/baouw/5.png" alt="" />
    </div>

    <div class="element">
      <img src="~/public/projects/baouw/6.png" alt="" />
    </div>

    <div class="element">
      <img src="~/public/projects/baouw/7.png" alt="" />
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

    &:nth-child(1), &:last-child {
      width: calc((100% / 3) * 2 - 30px);
    }

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;

    }

  }

}
</style>