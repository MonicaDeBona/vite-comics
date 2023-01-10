<script>
export default {
    name: 'AppHeader',
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
                    active: true,
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

<template>
    <div class="my-container">
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


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

    nav {
        width: 100%;
        height: 120px;
        display: flex;
        justify-content: space-between;
        align-items: center;

        ul {
            display: flex;
            justify-content: space-between;
            line-height: 120px;
            list-style-type: none;
            height: 100%;
            
            li {
                margin-left: 1.5rem;
                color: $nav-accent-color;
                font-weight: 700;
                height: 100%;
                
                &.active{
                    border-bottom: 5px solid $blue-color;
                }
            }
        }
    }

    .logo img {
            width: 80px;
        }
</style>