<template>
<section>
    <h1 v-if="prive === true">Level 10 :3</h1>
    <h1 v-if="likes > 0 "> This video has {{ likes }} </h1>
    <p v-else></p>
    <button v-on:click.capture="privety" v-on:click="likeAndSubs">Like & Subs</button>
</section>
</template>
<script>
export default {

}
</script>
<script>
export default {

    data() {
        return {
            likes: 1,
            prive: false
        }
    },

    methods: {
        likeAndSubs() {
            this.likes++;
        },

        privety() {
            if(this.likes > 11 ){
                this.prive === false; {
                    this.prive = true;
                }
            }
        }
    }
}
</script>