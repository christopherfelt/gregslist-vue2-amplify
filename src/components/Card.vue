<template>
    <b-card :style="cardStyle" align="center" class="p-0"  @click="clickHandler" v-b-hover="hoverHandler" :class="isHovered ? 'shadow-sm' : ''">
        <b-card-img class="p-1" :src="imgSrc"></b-card-img>
        <b-card-title>
            {{title}}
        </b-card-title>
        <b-card-text>
            {{description}}
        </b-card-text>
    </b-card>
</template>

<script>
export default {
    name: "CardComponent",
    data(){
        return{
            isHovered: false,

        }
    },
    props: {
        title: {
            type: String,
            default: "No Title"
        },
        description: {
            type: String,
            default: "No Description"
        },
        redirectUrl: String,
        cardStyle: String,
        imgSrc:{
            type: String,
            default: "https://placekitten.com/g/200/200"
        }
    },
    methods:{
        clickHandler(){
            this.$router.push(this.redirectUrl);
        },
        hoverHandler(hovered){
            this.isHovered = hovered
        }
    }
};
</script>

<style>
</style>