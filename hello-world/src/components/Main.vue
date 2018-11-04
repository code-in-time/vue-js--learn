<template>
    <div>
        this i the main template
        <br /><br />
        <AppFormInput :msg="m" @myMessageChanged="m = $event"></AppFormInput>
        <!-- <Message /> -->

    </div>
</template>

<script>
    import AppFormInput from "./AppFormInput.vue";
    // import Message from "./Message.vue";
    export default {
        data: () => {
            return {
                m: "my message"
            }
        },
        components: {
           AppFormInput,
        //    Message
       }

    }
</script>
