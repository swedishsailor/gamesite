<template>
    <div className="banner">
        <img :src=src />
        <div class="bannerContent">
        <h1>From ashes to empires. Your journey will shape the face of Verra. Experience an MMORPG where everything is permanently impacted</h1>
            <p>Experience an MMORPG where everything is permanently impacted
by your actions – explore, trade, build, and let the world take form. From your imagination through your will and into everyone's reality, what you create will be the cornerstone of the next explorer’s ambition.</p>
        </div>
    </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
    data(){
        return{

        }
    },
    setup(){
        const src = "https://i.postimg.cc/9MQfQD4M/8MRW.gif"
        return{
            src
        }
    }
})
</script>
<style lang="scss">
    .banner{
        min-width: 99vw;
        margin-top: 72px;
        display: flex;
       justify-content: center;
       text-align: center;
       .bannerContent{
        z-index: 25;
        position: absolute;
            color:#fff;
            width:50%;
     h1{
        margin-top: 15vh;
        font-family: 'Miltonian Tattoo', cursive;
        font-size:48px;
       }
       p{
        margin-top: 5vh;
        font-family: 'Poiret One', cursive;
        font-size:1.75rem;
       }
       }
        img{
            
            height: inherit;
            object-fit: cover;
        }
    }
</style>