<script>
export default {
    name: "AppJumbo",
}
</script>

<template>
    <section>
        <div class="container p-6">
            <div class="row">
                <div class="jumbotron jumbotron-fluid">
                    <div class="container">
                        <h1 class="welcome display-4 p-3">Welcome in my personal Portfolio</h1>
                        <p class="lead mt-3 p-3">Hi there! I'm Riccardo Grande,I have a small passion for computer science
                            and
                            electronics. Since I was young, I have always seen the web as one of the greatest inventions in
                            the world and I have always been curious about how web pages are created. I have learned some
                            of the main technologies, which you can see in the dedicated section. In addition to my
                            professional commitments, I enjoy playing video games when I can find some free time, although
                            unfortunately, I have little of it.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>



<style lang="scss" scoped>
.container {
    margin-top: 2rem;
    color: white;
    background-color: rgba(0, 0, 0, 0.19);
}

.welcome {

    font-family: 'Orbitron', sans-serif;
}

p {

    font-family: 'Play', sans-serif;
}
</style>