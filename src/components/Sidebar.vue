<template>

    <div class="sidebar">
        <h3 v-for="page in pages" class="pages">
            <i :class="'fa-xl fa-solid fa-fw ' + page.icon"></i>
            {{page.name}}
        </h3>
        <hr size="0.5" color="#363636">
        <p v-for="playlist in playlists" class="playlistItems">
            <a :href="playlist.link" target="_blank" rel="noreferrer noopener">{{playlist.name}}</a>
        </p>
    </div>

</template>

<script setup>

import {ref} from "vue"

let pages = [
    {name: "Home", icon: "fa-house"},
    {name: "Search", icon: "fa-magnifying-glass"},
    {name: "Your Library", icon: "fa-lines-leaning"},
    {name: "Create Playlist", icon: "fa-square-plus"},
    {name: "Liked Songs", icon: "fa-heart"}
]

let playlists = ref([
    // {name: "songs that remind me of chili 🙄", link: ""},
    {name: "i'll be the main antagonist", link: "https://open.spotify.com/playlist/5BzfSmyCHpdtILvAvSYfEH?si=6c644e9295e04ba5"},
    // {name: "stalking playlist", link: ""},
    {name: "please love me back", link: "https://open.spotify.com/playlist/0VMBPZ945sIieeQtEQeqF9?si=99a9918ac0964378"},
    {name: "moon-bound connection", link: "https://open.spotify.com/playlist/12GF3zySyMTd86armWIvzc?si=b41f24d875e8473c"},
    {name: "the band kid life", link: "https://open.spotify.com/playlist/3gCSs0cZilmq23kuKd71OQ?si=d588ad7ebaaa4b0a"},
    {name: "ugh tiktok", link: "https://open.spotify.com/playlist/17Vlprf6wC3hXSlKvHhzbX?si=8d060ebf538c4379"},
    {name: "oh to be young and in love", link: "https://open.spotify.com/playlist/0BPIIt13M3SPrw508lJkCq?si=c61be72dc2d74d2f"},
    {name: "i'm not a weeb i swear", link: "https://open.spotify.com/playlist/3kYgyPagBnv1hXcQsX0b78?si=9319c09fc9994963"},
    // {name: "wowow sparkly fuzzy uwuwu", link: ""},
    {name: "help me feel alive", link: "https://open.spotify.com/playlist/0EK60YpBav1A4EuKGBQc0A?si=310655c3c1ac4cd2"},
    {name: "hey comrade!", link: "https://open.spotify.com/playlist/66VbPvZOYblkG0Xw0ivahI?si=975455169e57408f"},
    {name: "i don't want to grow up", link: "https://open.spotify.com/playlist/2iHFJVyoLiGc5sRisCiCRn?si=b1169986f1fc4754"}
])

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
    font-size: 15px;
    z-index: 1;
}

.pages {
    cursor: default;
}

.pages i {
    margin-right: 15px;
}

.playlistItems a {
    text-decoration: none;
    color: grey;
    font-weight: bold;
    line-height: 25px;
}

.playlistItems a:hover {
    color: white;
}


</style>