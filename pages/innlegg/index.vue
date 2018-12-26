<template>
    <div class="innlegg">
        <h1 class="title">{{content.main.tittel}}</h1>
        <h3 class="author">Av {{content.author}}</h3>
        <p class="shortDescription">{{content.main.shortDesc}}</p>
        <div class="mainContent" v-html="content.main.body"></div>
    </div>
</template>

<style lang="scss">
div.innlegg {
    padding: 20px;
    @media screen and (min-width:760px) {        
        width: 80%;
        margin: 20px auto;
    }
    @media screen and (min-width:1400px) {        
        width: 60%;
        margin: 20px auto;
    }
    h1.title {
        font-weight: normal;
    }
    h3.author {
        font-weight: normal;
        margin-bottom: 10px;
    }
    p.shortDescription {
        font-style: italic;
    }
    div.mainContent {

    }
}
</style>

<script>
import innlegg from '~/assets/content/innlegg.json';
console.log('Innlegg',innlegg)

export default {
    asyncData({params}) {
        console.log(params);
        // Make dynamic
        let post = innlegg[0];
        console.log("Post ",post)
        return {
            content: post
        }
    }
}
</script>