<script>
export default {
    name: "AppHeader",
}
</script>

<template>
    <nav class="navbar navbar-dark bg-dark navbar-expand-lg justify-content-between p-3">
        <a class="navbar-brand" href="#">Riccardo Grande Web Developer</a>
        <div>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup"
                aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
                <div class="navbar-nav">
                    <router-link class="nav-item nav-link active" to="/">Home</router-link>
                    <router-link class="nav-item nav-link" to="/about">About</router-link>
                    <router-link class="nav-item nav-link" to="/contacts">Contact
                        me</router-link>

                </div>

            </div>

        </div>

    </nav>
</template>



<style lang="scss" scoped>
.navbar-brand {
    font-size: 2rem;
    font-family: 'Bebas Neue', sans-serif;
    color: white;
}

.navbar-collapse {
    color: white;
}
</style>