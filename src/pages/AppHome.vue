<script>
import axios from 'axios';

export default {
    name: "AppHome",
    data() {
        return {
            loading: true,
            projects: null,
            base_url: 'http://127.0.0.1:8000/',
            projects_path: 'api/projects',
            error: null
        }
    },
    methods: {
        getProjects(url) {

            axios.get(url)
                .then(response => {
                    console.log(response);
                    this.projects = response.data.projects
                    this.loading = false
                })
                .catch(error => {
                    console.log(error);
                    this.error = error.message
                })
        }
    },
    mounted() {

        const url = this.base_url + this.projects_path
        this.getProjects(url)

    }

}
</script>


<template>
    <h1>My Projects</h1>
    <section class="projects">
        <div class="container">
            <div class="row">
                <div class="col" v-if="projects">
                    <div class="card" v-for="project in projects">
                        <img class="card-img-top" src="" alt="">
                        <div class="card-body">
                            <h3>{{ project.title }}</h3>
                            <p>{{ project.content }}</p>
                        </div>

                    </div>
                </div>

            </div>
        </div>
    </section>
</template>



<style lang="scss" scoped></style>