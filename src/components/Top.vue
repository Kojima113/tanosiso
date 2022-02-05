<template>
    <div class="top">
        <!-- <button @click="goTop">
            便利屋 6 8
        </button> -->
        便利屋 6 8
    </div>
</template>

<script>
export default {
    el: "top",
    methods: {
        goTop: function() {
            this.$router.push('/')
        }
    }
}
</script>

<style scoped>
.top {
     background: linear-gradient(to right,#e60000,#f39800,#fff100,#009944,#0068b7,#1d2088,#920783);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    font-size: 500%;
    font-weight: bold;
    display: inline-block;
}
</style>