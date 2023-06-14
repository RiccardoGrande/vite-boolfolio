<script>
import axios from 'axios';

export default {
    components: {

    },
    data() {
        return {
            loading: true,
            projects: null,
            base_API: 'http://127.0.0.1:8000/',
            projects_path: 'api/projects'
        }
    },
    methods: {
        getProjects(url) {

            axios.get(url)
                .then(response => {
                    console.log(response);
                })
                .catch(error => {
                    console.log(error);
                })
        }
    },
    mounted() {

        const url = this.base_API + this.projects_path
        this.getProjects(url)

    }

}

</script>

<template>
    <section class="vue-home">
        <div class="container">
            <div class="row">

            </div>
        </div>
    </section>
</template>

<style lang="scss">
@use './styles/general.scss';
</style>
