<template>
    <div class="ssr-demo">
        <h2>Server-Side Rendered Data</h2>
        <p>{{ serverRenderedData }}</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            serverRenderedData: 'Data fetched on the server side!',
        };
    },
    mounted() {
        // Simulate fetching data from an API (you can replace this with actual API calls)
        // For simplicity, we use a timeout to simulate an asynchronous operation
        setTimeout(() => {
            // Update the server-rendered data after fetching
            this.serverRenderedData = 'Updated data from the server!';
        }, 2000);
    },
};
</script>

<style scoped>
.ssr-demo {
    padding: 20px;
    margin: 20px;
    border: 1px solid #ccc;
    border-radius: 4px;
}
</style>
