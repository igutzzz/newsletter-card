<template>
    <div class="topico">
        <p><img src="../assets/topic.png" alt="Tópico">{{ text }}</p>
    </div>
</template>

<script lang="ts">
    export default {
        props: {
            text: String,
        }
    }
</script>

<style scoped>

    .topico{
        margin: 1.5rem 0rem;
    }
    div p{
        display: flex;
        align-items: center;
        font-weight: 400;
    }

    img{
        margin-right: 0.5rem;
    }
</style>