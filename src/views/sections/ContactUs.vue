<template>
    <v-theme-provider dark>
        <base-section id="contact-us" class="contactus__section" space="40">
            <v-container>
                <v-row justify="center">
                    <v-col cols="10">
                        <base-title
                            class="my-6"
                            :space="$vuetify.breakpoint.mdAndUp ? 0 : 4"
                            title="Soyons partenaire"
                        />

                        <base-body space="0" class="my-6">
                            <span
                                class="white--text"
                            >Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolor itaque modi ab accusantium architecto voluptates ipsa molestiae.</span>
                        </base-body>
                        <base-btn
                            class="my-6"
                            :block="$vuetify.breakpoint.smAndDown"
                            color="white"
                            href="mailto:shop@vuetifyjs.com?subject=Zero%20Theme%20Question"
                            large
                            outlined
                            target="_blank"
                        >En savoir plus</base-btn>
                    </v-col>
                </v-row>
            </v-container>
        </base-section>
    </v-theme-provider>
</template>

<script>
export default {
    name: "SectionContactUs"
};
</script>

<style lang="scss">
.contactus__section {
    background-image: linear-gradient(
            to right,
            rgba(5, 11, 31, 0.6),
            rgba(5, 11, 31, 0.6)
        ),
        url("~@/assets/img/contactus.jpg");
    background-position: center; /* Center the image */
    background-repeat: no-repeat; /* Do not repeat the image */
    background-size: cover; /* Resize the background image to cover the entire container */
}
</style>
