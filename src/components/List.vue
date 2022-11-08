<template>
    <div>
        <h5><router-link to="/detail/0">{{ article[0].title }}</router-link></h5>
        <p>{{ article[0].date }}</p>
    </div>
    <div>
        <h5><router-link to="/detail/1">{{ article[1].title }}</router-link></h5>
        <p>{{ article[1].date }}</p>
    </div>
    <div>
        <h5><router-link to="/detail/2">{{ article[2].title }}</router-link></h5>
        <p>{{ article[2].date }}</p>
    </div>
</template>

<script>
export default {
    name: 'List',
    props: {
        article: Array,
    }
}
</script>

<style>

</style>