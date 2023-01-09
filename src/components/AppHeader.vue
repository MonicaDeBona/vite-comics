<template>
    <div class="container">
        <nav>
            <div class="logo">
                <img src="../assets/imgs/dc-logo.png" alt="DC main logo">
            </div>
            <ul>
                <li v-for="navItem in navItems" :class=" (navItem.active) ? 'active' : '' ">
                    {{ navItem.text }}
                </li>
            </ul>
        </nav>
    </div>
</template>

<script>
export default {
    data() {
        return {
            navItems: [
                {
                    text : "CHARACTERS",
                    url: "#",
                    active: false,
                },
                {
                    text : "COMICS",
                    url: "#",
                    active: false,
                },
                {
                    text : "MOVIES",
                    url: "#",
                    active: false,
                },
                {
                    text : "TV",
                    url: "#",
                    active: false,
                },
                {
                    text : "GAMES",
                    url: "#",
                    active: false,
                },
                {
                    text : "VIDEOS",
                    url: "#",
                    active: false,
                },
                {
                    text : "FANS",
                    url: "#",
                    active: false,
                },
                {
                    text : "NEWS",
                    url: "#",
                    active: false,
                },
                {
                    text : "SHOP",
                    url: "#",
                    active: false,
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

    div.container {
        width: 70%;
        height: 100%;
        margin: auto;
        display: flex;
        align-items: center;

        nav {
            width: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo img {
            width: 80px;
        }
    }

    nav ul {
        display: flex;
        justify-content: space-between;
        list-style-type: none;
        
        li {
            padding-right: 1.5rem;
            
            &.active,
            &:hover {
                color: $text-color1;
            }
        }
    }
</style>