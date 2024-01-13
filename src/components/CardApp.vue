
<script>
export default {
    name: 'CardApp',
    props: {
        card: Object
    },

}
</script>

<template lang="">
    <div >
        <img :src="card.thumb" alt="card.series" >
        <h5>{{card.series}}</h5>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/generals.scss' as *;



img {
    width: 100%;
    height: 150px;
    object-fit: inherit;
}

h5 {
    font-size: small;
    font-weight: bold;
    margin-top: 10px;
    color: white;
}
</style>