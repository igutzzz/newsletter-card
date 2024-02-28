<script setup lang="ts">
import EmailInput from "./components/EmailInput.vue";
import SendEmail from "./components/SendEmail.vue";
</script>

<template>
  <main>
    <div class="container">
      <div class="container__left-content">
        <h1 class="container__title">Fique por dentro!</h1>
        <p class="container__subtitle">
          Assine nossa newsletter e mantenha-se atualizado com:
        </p>
        <ul class="container__list">
          <li class="container__list-content">
            <img src="./assets/vector.png" />Promoções exclusivas
          </li>
          <li class="container__list-content">
            <img src="./assets/vector.png" />Conteúdos adicionais
          </li>
          <li class="container__list-content">
            <img src="./assets/vector.png" />+100 recursos grátis
          </li>
        </ul>
        <EmailInput />
        <SendEmail></SendEmail>
      </div>
      <div class="container__right-content">
        <img src="./assets/test-pc.png" alt="" />
      </div>
    </div>
  </main>
</template>

<style scoped>
@media (min-width: 800px) {
  main {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
  .container {
    background-color: #fcf7f8;
    min-width: auto;
    border-radius: 10px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 2em;
  }

  .container__left-content {
    margin-left: 2em;
  }

  .container__right-content {
    margin: 0em 2em;
    margin-left: 10px;
    border-radius: 10px;
    width: 45%;
    margin: 2em 0;
    margin-right: 2em;
  }

  .container__title {
    color: #226ce0;
    font-size: 36px;
    font-weight: 700;
  }

  .container__subtitle {
    color: #000000;
    font-size: 20px;
    font-weight: 400;
    line-height: 25px;
    width: 80%;
  }

  .container__list {
    display: inline-block;
    padding: 2em 0em;
    align-items: center;
  }

  .container__list img {
    height: 2em;
    width: 2em;
    margin-right: 1em;
  }

  .container__list-content {
    display: flex;
    align-items: center;
    list-style-type: none;
    text-decoration: none;
    margin: 1em 0;
  }

  .container__right-content img {
    width: 100%;
  }
}

  @media (max-width: 800px) {
    ul {
      padding-inline-start: 0px;
    }
    
    main {
      height: 100%;
      width: 100%;
      justify-content: center;
      background-color: #FFFFFF;
    }
    
    .container {
      display: flex;
      flex-direction: column-reverse;
      align-items: center;
      width: 100%;
    }
    
    .container__right-content {
      height: auto;
    }

    .container__right-content img {
      width: 100vw ;
      border-radius: 0px 0px 20px 20px;
      height: 350px;
    }

    .container__left-content {
      display: flex;
      flex-direction: column;
    }

    .container__title {
    color: #226ce0;
    font-size: 30px;
    font-weight: 700;
    }
    
    .container__subtitle {
    color: #000000;
    font-size: 16px;
    font-weight: 400;
    }

    .container__list {
    display: inline-block;
    align-items: center;
    margin: 10px 0px;
    }

    .container__list img {
    height: 26px;
    width: 26px;
    margin: 5px 0px;
    margin-right: 10px;
    }

    .container__list-content {
    display: flex;
    align-items: center;
    list-style-type: none;
    text-decoration: none;
    margin: 8px 0;
    }
  }
</style>
