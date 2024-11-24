<template>
    <header>
        <nav>
            <ul>
                <li><NuxtLink to="/">Index</NuxtLink></li>
                <li><NuxtLink to="/about">About</NuxtLink></li>
                <!-- <li><NuxtLink to="/posts/{ $route }">Nothing</NuxtLink></li> -->
            </ul>
        </nav>
    </header>
    <div>
        <p class="default-layout">Default layout</p>
        <slot></slot>
    </div>
</template>

<style>
.default-layout {
    color:blueviolet
}
</style>