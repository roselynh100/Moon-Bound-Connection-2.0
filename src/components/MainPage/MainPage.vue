<template>

    <div class="mainPage">
        <div class="mainPageContent">
            <Profile />
            <p>there is nothing here</p>
        </div>
    </div>

</template>

<script setup>

import Profile from './Profile.vue'


</script>

<style>

.mainPage {
    width: 100%;
    height: 1000vh;
    top: 0;
    left: 0;
    position: absolute;
}

.mainPageContent {
    margin-left: calc(20vw + 70px);
    background-color: purple;
}

</style>