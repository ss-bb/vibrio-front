<template>
    <v-theme-provider dark>
        <base-section id="contact-us" class="contactus__section" space="80">
            <v-container>
                <v-row justify="center">
                    <v-col cols="10">
                        <base-heading
                            class="my-6"
                            :space="$vuetify.breakpoint.mdAndUp ? 0 : 4"
                            title="Soyons partenaire"
                        />

                        <div class="contactus__div-limit">
                            <base-body space="0" class="my-6">
                                <span
                                    class="white--text"
                                >Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem</span>
                            </base-body>
                        </div>
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

.contactus__div-limit {
    width: 70%;
}
</style>
