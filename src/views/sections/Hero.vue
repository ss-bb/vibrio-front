<template>
    <section id="hero">
        <v-img
            :min-height="minHeight"
            :src="require('@/assets/img/home-vibrio.jpg')"
            class="white--text"
            gradient="to right, rgba(5, 11, 31, .5), rgba(5, 11, 31, .5)"
        >
            <v-container class="fill-height px-4 py-12">
                <v-responsive
                    class="d-flex align-center"
                    height="100%"
                    max-width="700"
                    width="100%"
                >
                    <base-heading
                        class="ml-12"
                        size="display-1"
                        title="Nous concevons des événements médicaux"
                    />
                    <base-heading class="ml-12" size="display-1" title="Mais autrement" />
                </v-responsive>
            </v-container>
        </v-img>
    </section>
</template>

<script>
export default {
    name: "SectionHero",

    provide: {
        theme: { isDark: true }
    },

    computed: {
        minHeight() {
            const height = this.$vuetify.breakpoint.mdAndUp ? "100vh" : "50vh";
            return `calc(${height})`;
        }
    }
};
</script>
