<script setup lang="ts">
defineProps({
  title : String,
  text1 : String,
  text2 : String,
})
</script>

<template>
  <div class="projectPageTitle">
    <span class="line"></span>
    <div class="content">
      <h1>{{ title }}</h1>
      <p> {{ text1 }} </p>
      <p> {{ text2 }} </p>
    </div>
  </div>
</template>

<style scoped lang="scss">
.projectPageTitle {
  display: flex;
  color: white;
  margin: 4rem 0;

  .line {
    background: white;
    width: 18%;
    height: 1px;

  }

  .content {
    margin-left: 1rem;

    h1 {
      color: #FFFFFF;
      font-size: 25px;
      font-weight: 900;
      transform: translateY(-50%);

    }

    p {
      font-size: 15px;
      margin: .5rem 0;

    }

  }

}
</style>