<template>
    <div>
        main2 template {{message}}
        <appInput :msg="message" @evMessageChange="message = $event"></appInput>

    </div>
</template>

<script>
    import appInput from "./appInput.vue";
    // import Messagessss from "./Message.vue";
    export default {

        data: () => {
            return {
                message: "my message"
            }
        },
        components: {
           appInput,
        //    Message
       }

    }
</script>
