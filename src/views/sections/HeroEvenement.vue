<template>
    <section id="hero">
        <v-img
            :min-height="minHeight"
            :src="require('@/assets/img/event-hero.jpg')"
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
                    <base-title class="mx-12" title="Next." />
                    <base-heading
                        class="mx-12 my-3"
                        title=" Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi fermentum maximus purus, eget consectetur massa ultricies ac. In porttitor neque in leo pharetra, at pharetra massa dictum. Donec sollicitudin non ex at tincidunt. Cras tincidunt nisl leo, vel facilisis lorem auctor eu. Donec eget viverra magna, eget pulvinar sem."
                    />
                    <div>
                        <base-btn color="accent">Réservez</base-btn>
                        <base-btn color="accent">Découvrez</base-btn>
                    </div>
                </v-responsive>
            </v-container>
        </v-img>
    </section>
</template>

<script>
export default {
    name: "SectionHeroEvenement",
    provide: {
        theme: { isDark: true }
    },
    computed: {}
};
</script>
