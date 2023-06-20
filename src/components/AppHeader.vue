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
                    <a class="nav-item nav-link active" href="../pages/AppHome.vue"><router-link
                            to="/">Home</router-link></a>
                    <a class="nav-item nav-link" href="../pages/AppAbout.vue"><router-link
                            to="/about">About</router-link></a>
                    <a class="nav-item nav-link" href="../pages/AppContacts.vue"><router-link to="/contacts">Contact
                            me</router-link></a>

                </div>

            </div>

        </div>

    </nav>
    <router-view></router-view>
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