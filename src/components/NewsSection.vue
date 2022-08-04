<script>
import { defineComponent } from "vue"
export default defineComponent({
    data() {
        return {

        }
    },
    setup() {
        const news = [{ src: 'https://i.postimg.cc/GpVQqK3v/1200x630-grafika.webp', title: 'Nowy bohater Krzys', content: 'At vero eos et accusamus et' },
        { src: 'https://i.postimg.cc/GpVQqK3v/1200x630-grafika.webp', title: 'Patch 4.0.3 preview', content: 'At vero eos et accusamus et' },
        { src: 'https://i.postimg.cc/GpVQqK3v/1200x630-grafika.webp', title: 'IEM Katowice 2022', content: 'At vero eos et accusamus et' }]
        console.log(news)
        return {
            news
        }
    }
})
</script>
<template>
    <div class="news">
        <h1 class="header">News</h1>
        <ul>
            <li><img :src=news[0].src />
                <h1>{{ news[0].title }}</h1>
                <p>{{ news[0].content }}</p>
            </li>
            <li><img :src=news[1].src />
                <h1>{{ news[1].title }}</h1>
                <p>{{ news[1].content }}</p>
            </li>
            <li><img :src=news[2].src />
                <h1>{{ news[2].title }}</h1>
                <p>{{ news[2].content }}</p>
            </li>
        </ul>
    </div>
</template>
<style lang="scss">
.news {
    background-color: #4A588D;
    display: flex;
    flex-direction: column;
    padding-top: 5px;

    .header {
        text-align: center;
        font-size: 96px;
        font-family: 'Cormorant SC', serif;
        color: rgb(7, 7, 7);
        letter-spacing: 5px;
        z-index: 20;
        text-shadow: -2.5px 2.5px 0px #4af844, -5px 5px 0px #000000;
        margin-bottom: 35px;
    }

    ul {
        list-style: none;
        display: flex;
        flex-direction: row;
        height: inherit;
        margin: auto;
        padding-bottom: 105px;

        li {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin: 15px;
            height: 105px;
            justify-content: space-around;

            h1 {
                margin-top: 17.5px;
                font-size: 24px;
            }

            img {
                width: 335px;
                height: 335px;
            }

            p {
                margin-top: 8.5px;
            }
        }
    }
}
</style>