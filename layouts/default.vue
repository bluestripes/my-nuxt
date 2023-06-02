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
        <div>
            <slot />
        </div>
    </div>
</template>

<style scoped>
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    ul {
        
    }

    .router-link-exact-active {
        color: red;
    }
</style>