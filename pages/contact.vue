<script setup lang="ts">
</script>

<template>
  <div class="contact">
    <div class="form">
      <h1>Réalisons vos projets ensemble !</h1>
      <p>Utilisez le formulaire ou envoyez un e-mail à maurine.callot74@gmail.com</p>
      <form action="">
        <div>
          <label for="name">
            <span>Nom</span>
            <input name="name" id="name" type="text"></input>
          </label>
          <label for="pname">
            <span>Prénom</span>
            <input name="pname" id="pname" type="text"></input>
          </label>
        </div>
        <div>
          <label for="mail">
            <span>Adresse mail</span>
            <input name="mail" id="mail" type="text"></input>
          </label>
        </div>
        <div>
          <label for="msg">
            <span>Message</span>
            <textarea name="msg" id="msg"></textarea>
          </label>
        </div>
      </form>
    </div>
    <div class="img">
      <img src="/contact.png" alt="">
    </div>
  </div>
</template>

<style scoped>
.contact {
  color: white;
  display: flex;
  padding: 72px;
  
  @media screen and (max-width: 1065px) {
    padding: 32px;
  }
  @media screen and (max-width: 817px) {
    flex-direction: column;
    align-items: center;
    gap: 30px;
  }

  .form {
    width: 60%;
    display: flex;
    flex-direction: column;
    @media screen and (max-width: 817px) {
      width: 100%;
    }

    h1 {
      font-size: 25px;
      font-weight: bold;
      margin-bottom: 10px;

      @media screen and (max-width: 1065px) {
        font-size: 20px;
      }

    }

    p {
      font-size: 15px;
      font-weight: lighter;
      margin-bottom: 30px;

      @media screen and (max-width: 1065px) {
        font-size: 14px;
      }

    }

    form {
      padding-right: 72px;
      display: flex;
      flex-direction: column;
      height: 100%;
      gap: 34px;

      @media screen and (max-width: 1065px) {
        padding-right: 32px;
      }
      @media screen and (max-width: 817px) {
        padding-right: 0;
      }

      & > div {

        display: flex;
        gap: 24px;
        @media screen and (max-width: 1065px) {
          gap: 12px;
        }

        label {
          width: 100%;
          display: flex;
          flex-direction: column;
          position: relative;

          span {
            margin-bottom: 8px;
            font-size: 20px;
            font-weight: 700;
            @media screen and (max-width: 1065px) {
              font-size: 16px;
            }

          }

          input, textarea {
            color: black;
            font-size: 20px;
            outline: none;
            padding: 6px;
            width: 100%;
            @media screen and (max-width: 1065px) {
              font-size: 16px;
              padding: 5px;
              width: calc(100% - 10px);
            }

          }

        }

        &:last-child {
          height: 100%;

          textarea {
            height: 100%;

          }

        }

      }

    }

  }

  .img {
    width: 40%;
    display: flex;
    justify-content: flex-end;
    @media screen and (max-width: 817px) {
      width: 60%;
    }

    @media screen and (max-width: 1290px) {
      img {
        width: 100%;
        object-fit: cover;
        object-position: center;

      }
    }

  }

}
</style>