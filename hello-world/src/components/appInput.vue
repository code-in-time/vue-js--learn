<template>
    <div>
        appInput.vue {{msg}}
        <input type="text" :value="msg" @input="changeNessage" />
        {{ message }}

    </div>
</template>

<script>
    export default {
        props: [ 'msg' ],
        data: () => {
            return {
                message: "my message"
            }
        },
        methods: {
            changeNessage(e) {
                this.message = e.target.value;
                this.$emit('evMessageChange', this.message)
            }
        }

    }
</script>
