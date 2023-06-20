<script>
import AppHeader from './components/AppHeader.vue'
import AppJumbo from './components/AppJumbo.vue'

export default {
    components: {

        AppHeader,
        AppJumbo
    }
}
</script>

<template>
    <video id="background-video" autoplay muted loop>
        <source src="./assets/pexels-engin-akyurt-2963870-3840x2160-25fps.mp4" type="video/mp4">

    </video>
    <AppHeader></AppHeader>
    <AppJumbo></AppJumbo>
    <router-view></router-view>
</template>

<style lang="scss">
@use './styles/general.scss';

#background-video {
    position: fixed;
    right: 0;
    bottom: 0;
    min-width: 100%;
    min-height: 100%;
    width: auto;
    height: auto;
    z-index: -1;
}
</style>
