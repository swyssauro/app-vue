<template>
   <div class="container">
    <b-jumbotron>
    <template v-slot:header>BootstrapVue</template>

    <template slot="lead">
        {{ currentQuestion.question }}
    </template>

    <hr class="my-4">

   <b-list-group>
        <b-list-group-item
        v-for="(answers, index) in answers"
        :key="index"
        >
        {{answers}}
        </b-list-group-item>
    </b-list-group>

    <b-button variant="primary" href="#">Do Something</b-button>
    <b-button @click="next" variant="success" href="#">Prox</b-button>
  </b-jumbotron>
</div>
</template>
<script>
export default {
    props: {
        currentQuestion: Object,
        next: Function
    },
    computed: {
        answers() {
            let answers = [...this.currentQuestion.incorrect_answers]
            answers.push(this.currentQuestion.correct_answer)
            return answers
        }
    },
    mounted() {
        console.log(this.currentQuestion)
    }
}
</script>