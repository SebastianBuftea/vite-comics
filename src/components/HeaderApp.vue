<script>
export default {
    name: 'HeaderApp',
    data() {
        return {
            links: [
                {
                    label: 'characters',
                    url: '#',
                    current: true,
                },
                {
                    label: 'comics',
                    url: '#',
                    current: false,
                },
                {
                    label: 'movies',
                    url: '#',
                    current: false,
                },
                {
                    label: 'tv',
                    url: '#',
                    current: false,
                },
                {
                    label: 'games',
                    url: '#',
                    current: false,
                },
                {
                    label: 'collectibles',
                    url: '#',
                    current: false,
                },
                {
                    label: 'videos',
                    url: '#',
                    current: false,
                },
                {
                    label: 'fans',
                    url: '#',
                    current: false,
                },
                {
                    label: 'news',
                    url: '#',
                    current: false,
                },
                {
                    label: 'shop',
                    url: '#',
                    current: false,
                },
            ]

        }
    },

}
</script>
<template lang="">

    <header>
        <img src="../assets/vue-dc-comics-1/img/dc-logo.png" alt="dc_logo">
        <nav>
          <ul>
            <li v-for="(link, index) in links" :key="index">
                <a :class="link.current ? 'active' : ''" :href="link.url">
                    {{link.label}}
                </a>
            </li>
          </ul>
        </nav>
    </header>

</template>

<style lang="scss">
header {
    display: flex;
    justify-content: space-between;
    margin: 10px 100px;

    ul {
        list-style: none;

    }

}
</style>