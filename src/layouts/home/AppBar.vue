<template>
    <div>
        <v-app-bar id="home-app-bar" app elevation="1" height="80" class="appbar__home">
            <base-img
                :src="require('@/assets/img/logo.svg')"
                class="mr-3 hidden-md-and-up"
                contain
                max-width="52"
                width="100%"
                height="80px"
            />

            <base-img
                :src="require('@/assets/img/vibrio-logo-light.svg')"
                contain
                max-width="128"
                width="100%"
                height="80px"
            />

            <v-spacer />

            <div>
                <v-tabs class="hidden-sm-and-down tabs__appbar" optional hide-slider>
                    <v-tab
                        v-for="(name, i) in items"
                        :key="i"
                        :to="{ name }"
                        :exact="name === 'Home'"
                        :ripple="false"
                        active-class="primary--text"
                        class="font-weight-bold white--text"
                        min-width="96"
                        text
                    >{{ name }}</v-tab>
                </v-tabs>
            </div>

            <v-app-bar-nav-icon class="hidden-md-and-up" @click="drawer = !drawer" />
        </v-app-bar>

        <home-drawer v-model="drawer" :items="items" />
    </div>
</template>

<script>
export default {
    name: "HomeAppBar",

    components: {
        HomeDrawer: () => import("./Drawer")
    },

    data: () => ({
        drawer: null,
        items: [
            "Home",
            "Agence",
            "Ambition",
            "Partenaire",
            "Team",
            "Contact",
            "Pro",
            "About"
        ]
    })
};
</script>

<style lang="sass">
#home-app-bar
.v-tabs-slider
    max-width: 24px
    margin: 0 auto

    .v-tab
    &::before
        display: none

.theme--light.v-tabs > .v-tabs-bar
    background-color: transparent
</style>

<style lang="scss" scoped>
.appbar__home {
    background-color: transparent !important;
}
</style>
