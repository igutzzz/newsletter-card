<template>
    <div>
        <label for="email">E-mail</label>
        <br>
        <input type="email" name="email" id="email" placeholder="Digite o seu e-mail">
    </div>
</template>

<script lang="ts">
    export default {
        
    }
</script>

<style scoped> 
    /* Estilizar o input de e-mail */
    input {
        border: 1px solid #D0D5DD;
        border-radius: 10px;
        outline: none;
        margin-bottom: 1.5rem;
        padding: 0.9rem;
        font-weight: 500;
        width: 100%;
    }

    label{
        font-size: 0.8rem;
        font-weight: 400;
    }

    input label{
        font-family: "Inter";
        font-weight: 500;
        font-size: 0.8rem;
    }

    input:focus{
        border: 1px 1px #D0D5DD;
    }
</style>