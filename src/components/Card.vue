<template>
<div @click="clickHandler" v-b-hover="hoverHandler" :class="isHovered ? 'shadow-sm' : ''">
    <b-card style="height: 200px" align="center" class="pt-4">
        <b-card-title>
            {{title}}
        </b-card-title>
        <b-card-text>
            {{description}}
        </b-card-text>
    </b-card>
</div>
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
        redirectUrl: String
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