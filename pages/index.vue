<template>
    <Head>
        <Title>Index page</Title>
    </Head>
    <div>
        <h1 class="m-2 border border-black">Welcome to the homepage</h1>
        <AppAlert>
            This is an auto-imported component
        </AppAlert>
    </div>

    <div v-if="data == null">
        No data
    </div>
    <div v-else>
        <ul v-for="post in data">
            <li>{{ post.title }}, {{ post.body }}</li>
        </ul>
    </div>
</template>

<script setup lang="ts">
const { data } = await useFetch('http://localhost:8000/api/posts/')
</script>