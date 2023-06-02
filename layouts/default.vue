<template>
    <div>
        <header>
            <NuxtLink to="/">Site title</NuxtLink>
            <nav>
                <ul>
                    <li><NuxtLink to="/">Home</NuxtLink></li>
                    <li><NuxtLink to="/about">About</NuxtLink></li>
                    <li><NuxtLink to="/user">User</NuxtLink></li>
                    <li><NuxtLink to="/document/123">Document</NuxtLink></li>
                </ul>
            </nav>
        </header>

        <!-- page content -->
        <div class="content">
            <slot />
        </div>
    </div>
</template>

<style scoped>
    html, body { margin: 0;padding: 0;}
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color:cadetblue;
        padding: 0 12px;
        box-shadow: 1px 1px 2px black;
    }
    ul {
        display: flex;
        list-style: none;
        gap: 12px;
    }

    .content { padding: 12px;}

    .router-link-exact-active {
        color: red;
    }
</style>