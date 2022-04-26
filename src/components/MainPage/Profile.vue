<template>

    <div class="profile">
        <a>Thunder 78</a>
        <i class="fa-solid fa-xl fa-caret-down"></i>
    </div>

    

</template>

<script setup>
</script>

<style>

.profile {
    position: fixed;
    right: 10px;
    background-color: black;
    color: white;
    font-weight: bold;
    padding: 5px 30px;
    border: solid black;
    border-radius: 100px;
    height: 30px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.profile:hover {
    background: #282828;
    border-color: #282828;
    cursor: pointer;
}

</style>