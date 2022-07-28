<script setup lang="ts">
import EcosystemIcon from './icons/IconEcosystem.vue'
</script>
<template>
    <div class="navbar">
        <EcosystemIcon id="logo"/>
        <ul className="navbarList">
            <li>Download</li>
            <li>Library</li>
            <li>Community</li>
            <li>Highscores</li>
            <li>Forum</li>
        </ul>
    </div>
</template>
<style lang="scss">
.navbar {
    z-index: 20;
    position: fixed;
    top: 0;
    width: 100%;
    text-align: center;
    display: flex;
    justify-content: center;
    background-color: #000;
    #logo{
        margin-block:auto;
        color:red;
    }
    .navbarList {
    list-style: none;
    display: flex;
    flex-direction: row;
    padding: 12.5px;
    li {
        border-radius: 10px;
        font-size: 18px;
        margin-inline: 20px;
        padding:10px;
        cursor: pointer;
        &:hover{
            background-color: rgba(255,255,255,0.1);
        }
    }
}
}
</style>