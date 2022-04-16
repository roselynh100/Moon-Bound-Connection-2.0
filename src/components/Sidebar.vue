<template>

    <div class="sidebar">
        <h3 v-for="page in pages" class="pages">
            {{page}}
        </h3>
        <hr size="0.5" color="#363636">
        <p v-for="playlist in playlists" class="playlistItems">
            {{playlist}}
        </p>
    </div>

</template>

<script setup>

import {ref} from "vue"

let pages = [
    "Home",
    "Search",
    "Your Library",
    "Create Playlist",
    "Liked Songs"
]

let playlists = ref([
    "songs that remind me of chili 🙄",
    "stalking playlist",
    "moon-bound connection",
    "the band kid life",
    "oh to be young and in love",
    "i'm not a weeb i swear",
    "wowow sparkly fuzzy uwuwu",
    "hey comrade!",
    "extra"])

</script>

<style>

.sidebar {
    background-color: black;
    color: grey;
    width: 20vw;
    height: 100vh;
    padding: 2px 30px;
    top: 0;
    left: 0;
    position: fixed;
}

.pages {
    margin-left: 75px;
}

.playlistItems {
    font-weight: bold;
}

.playlistItems:hover {
    color: white;
    cursor: pointer;
}


</style>