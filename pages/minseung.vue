<template>
    <div>
        <h2>Hello world</h2>
        <h3>{{message}}</h3>
        {{fullName}}
    </div>
</template>

<script lang="ts">
    import Vue from 'vue'

    export default Vue.extend({
        data(){
            return {
                message : 'Hello World',
                firstname : 'minseung',
                lastname : 'Park'
            }
        },
        computed: {
            fullName (): string {
                return `${this.firstname} ${this.lastname}`
            }
        }
    })
</script>

<style scoped>

</style>