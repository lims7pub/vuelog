<template>
    <article>
        <img src="https://cdn.pixabay.com/photo/2014/04/13/20/49/cat-323262_960_720.jpg" class="img-fluid mt-5 mb-5" alt="">
        <h2>{{ article[$route.params.id].title }}</h2>
        <p class="text-start mt-3">{{ article[$route.params.id].content }}.</p>
    </article>
</template>

<script>
export default {
    name: 'Detail',
    props: {
        article: Array,
    }
}
</script>

<style>

</style>