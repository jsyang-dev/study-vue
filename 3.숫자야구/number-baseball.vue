<template>
    <div>
        <h1>{{result}}</h1>
        <form v-on:submit="onSubmitForm">
            <input ref="answer" maxlength="4" v-model="value"/>
        </form>
    </div>
    <div>시도: {{}}</div>
</template>

<script>
    export default {
        data() {
            return {
                value: '',
                result: ''
            }
        },
        methods: {
            onSubmitForm(e) {
                e.preventDefault();
            }
        }
    };
</script>

<style>

</style>