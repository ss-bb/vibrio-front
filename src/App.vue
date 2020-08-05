<template>
    <v-fade-transition mode="out-in">
        <router-view />
    </v-fade-transition>
</template>

<script>
export default {
    name: "App",
    metaInfo: {
        title: "App",
        titleTemplate: "%s | Vibrio",
        htmlAttrs: { lang: "fr" },
        meta: [
            { charset: "utf-8" },
            { name: "viewport", content: "width=device-width, initial-scale=1" }
        ]
    }
};
</script>

<style lang="sass">
.extra-padding
    padding-bottom: 96px !important
    padding-top: 96px !important
</style>
