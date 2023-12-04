<template>
    <h1>
        Hello world!
    </h1>
</template>
<script>
import axios from "axios";

export default {
    mounted() {
        this.test();
    },
    methods: {
        async test() {
            const responseTest = await axios.get('/test');
            console.log(responseTest);
        }
    }
}
</script>
