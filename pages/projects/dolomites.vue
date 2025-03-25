<script setup lang="ts">

</script>

<template>
  <project-page-title
      title="DOLOMITES"
      text1=""
      text2="Edit : MC Production"
  />

  <div class="galerie">

    <div class="col">
      <div class="element">
        <img src="~/public/projects/dolomites/1.png" alt="" />
      </div>
      <div class="row">
        <div class="element">
          <img src="~/public/projects/dolomites/2.png" alt="" />
        </div>

        <div class="element">
          <img src="~/public/projects/dolomites/3.png" alt="" />
        </div>
      </div>
    </div>
    <div class="col">
      <div class="element">
        <img src="~/public/projects/dolomites/4.png" alt="" />
      </div>

      <div class="element">
        <img src="~/public/projects/dolomites/5.png" alt="" />
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
    gap: 30px;
    height: 100%;

    &:nth-child(1) { width: calc(70% - 30px); }
    &:nth-child(2) {
      width: calc(30% - 30px);
      .element {
        &:nth-child(1) { height: calc(70% - 30px); }
        &:nth-child(2) { height: calc(30% - 30px); }

      }
    }

    .row {
      display: flex;
      gap: 30px;

    }
  }

  .element {
    width: 100%;

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;

    }

  }

}
</style>