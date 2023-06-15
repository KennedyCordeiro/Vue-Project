<script setup>
import {ref} from 'vue';

function login() {
    console.log('teste login', email.value, password.value);
}

const email = ref('');
const password = ref('');

</script>

<template>
    {{email}}

    <form action="" @submit.prevent="login">
        <input type="text" placeholder="Email" v-model="email">
        <input type="text" placeholder="Password" v-model="password">
        <button type="submit">Login</button>
    </form>
</template>

<style></style>