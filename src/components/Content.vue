<template>
    <section class="container">
        <div class="content">
            <div class="content__texts">
                <h1 class="title">Fique por dentro!</h1>
                <p class="text">Assine nossa newsletter e mantenha-se atualizado com:</p>
                <Topics text="Promoções exclusivas"/>
                <Topics text="Conteúdos adicionais"/>
                <Topics text="+100 recursos grátis"/>
            </div>
            <div class="content__buttons">
                <EmailInputVue/>
                <SubscribeBtn/>
            </div>
        </div>
        <img src="../assets/computer.png" alt="Computador"> 
    </section>
</template>

<script lang="ts">
import EmailInputVue from './EmailInput.vue';
import SubscribeBtn from './SubscribeBtn.vue';
import Topics from './Topics.vue';

    export default{
    components: { EmailInputVue, SubscribeBtn, Topics }
}
</script>

<style scoped>  
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
    .container{
        display: flex;
        padding: 1rem;
        background-color: #FCF7F8;
        border-radius: 0.6rem;
    }
    .title{
        color: #226CE0;
        font-size: 2.2rem;
        font-family: "Inter";
        font-weight: 700;
        margin: 0.8rem 0;
    }
    .text{
        color: #000;
        font-size: 1rem;
        font-family: "Inter";
        font-weight: 400;
        margin: 0 0 14px 0;
    }

    .content{
        margin-right: 1.5rem;
    }

    .container__image{
        margin: 0;
    }

    .content__buttons{
        margin: 0;
        width: 100%;
    }
    .content__texts{
        display: column;
        width: 19.7rem;
    }

    section div{
        margin: 0 2.6rem 0 1rem;
    }

    ul li{
        margin: 0 0 20px 0;
        list-style-image: url("../assets/topic.png");
        font-family: "Inter";
        font-weight: 400;
        color: #000;
    }

    img{
        width: 18.8rem;
        height: 29.6rem;
    }

    @media (max-width: 760px){
        .container{
            display: flex;
            flex-direction: column-reverse;
            width: 100vw;
            height: 100vh;
            padding: 0;
            padding-bottom: 5rem;
        }

        .content{
            margin: 0 auto;
        }
        .container__buttons{
            width: 19.7rem;
        }

        img{
            width: 100%;
            border-radius: 0 0 20px 20px;
        }
    }
</style>    