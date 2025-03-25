<script setup lang="ts">
</script>

<template>
  <project-page-title
      title="PARC DU MERLET"
      text1=""
      text2="Edit : MC Production"
  />

  <div class="galerie">

    <div class="col">
      <div class="element">
        <img src="~/public/projects/merlet/1.png" alt="" />
      </div>

      <div class="element">
        <img src="~/public/projects/merlet/2.png" alt="" />
      </div>
    </div>

    <div class="col">
      <div class="element">
        <img src="~/public/projects/merlet/3.png" alt="" />
      </div>

      <div class="element">
        <img src="~/public/projects/merlet/4.png" alt="" />
      </div>
    </div>

    <div class="col">
      <div class="element">
        <img src="~/public/projects/merlet/5.png" alt="" />
      </div>

      <div class="element">
        <img src="~/public/projects/merlet/6.png" alt="" />
      </div>
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
  height: 200vh;

  .col {
    display: flex;
    flex-direction: column;
    width: calc(100% / 3 - 30px);
    height: 100%;
    gap: 30px;

    &:nth-child(1) , &:nth-child(3) {
      .element {
        &:nth-child(1) {
          height: calc(70% - 30px);

        }
        &:nth-child(2) {
          height: calc(30% - 30px);

        }
      }
    }

    .element {
      width: 100%;

      img {
        width: 100%;
        height: 100%;
        object-fit: cover;

      }

      &:nth-child(1) {
        height: calc(30% - 30px);

      }
      &:nth-child(2) {
        height: calc(70% - 30px);

      }

    }


  }

}
</style>