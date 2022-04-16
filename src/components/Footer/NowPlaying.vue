<template>

    <div class="nowPlaying">
        <img src="https://data.whicdn.com/images/227032586/original.gif" alt="square icon" id="nowPlayingIcon">
        <div class="nowPlayingInfo">
            <p>now playing!!!!</p>
            <p>now playing ARTIST!</p>
        </div>
    </div>

</template>

<script setup>
</script>

<style>

.nowPlaying {
    padding: 12px 0;
    display: flex;
}

#nowPlayingIcon {
    max-width: 100%;
    max-height: 100%;
}

.nowPlayingInfo {
    font-weight: bold;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 12px;
}

.nowPlayingInfo p {
    margin: 0;
}

</style>