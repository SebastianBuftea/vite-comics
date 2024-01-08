<script>
export default {
    name: 'HeaderApp',
    data() {
        return {
            links: [
                {
                    label: 'Characters',
                    url: '#',
                    current: true,
                },
                {
                    label: 'Comics',
                    url: '#',
                    current: false,
                },
                {
                    label: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    label: 'Tv',
                    url: '#',
                    current: false,
                },
                {
                    label: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    label: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    label: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    label: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    label: 'News',
                    url: '#',
                    current: false,
                },
                {
                    label: 'Shop',
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
@use '../styles/partials/variables' as *;

header {
    display: flex;
    justify-content: space-between;
    margin: 10px 100px;
    font-size: xx-small;

    img {
        width: 60px;
    }

    nav {
        display: flex;
        align-items: center;

        ul {
            list-style: none;
            display: flex;

            li {
                margin: 0px 10px;
                text-decoration: none;

                a {
                    text-decoration: none;
                    color: black;

                    &.active {
                        color: $primary_color;
                    }
                }
            }
        }
    }
}
</style>