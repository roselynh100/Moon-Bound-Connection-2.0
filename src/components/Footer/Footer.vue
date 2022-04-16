<template>

    <div class="footer">
        <NowPlaying />
        <Controls />
        <Volume />
    </div>

</template>

<script setup>

import Controls from './Controls.vue'
import NowPlaying from './NowPlaying.vue'
import Volume from './Volume.vue'

</script>

<style>

.footer {
    background-color: #1B1B1B;
    color: white;
    width: calc(100% - 30px);
    height: 90px;
    position: fixed;
    left: 0;
    bottom: 0;
    z-index: 100;
    padding: 0 15px;
    display: flex;
    justify-content: space-between;
}

</style>
