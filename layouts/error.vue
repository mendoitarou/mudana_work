<template>
    <div id="error">
        <div>
            <p v-if="status === 404">
                404 Not Found<br>
            </p>
            <p v-else>Error: {{ status }}</p>
            <NuxtLink to="/">Return Top</NuxtLink>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        error: {
            type: Object,
            default: null
        }
    },
    computed: {
        status() {
            return this.error.statusCode;
        }
    }
};
</script>
