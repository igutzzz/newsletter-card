<template>
    <div>
        <label for="email">E-mail</label>
        <input type="email" name="email" id="email" placeholder="Digite o seu e-mail">
    </div>
</template>

<script lang="ts">
    export default {
        
    }
</script>

<style scoped> 
    /* Estilizar o input de e-mail */
    label {
        font-weight: 500;
        color: black;
        display: block;
    }
    input {
        border-color: #D0D5DD;
        border: 2px solid;
        padding: 10px 14px;
        outline: none;
        background-color: transparent;
        border-radius: 10px;
        color: #667085;
        font-weight: 400;
        font-size: 14px;
        margin-top: 8px;
        min-width: 300px;
    }
</style>