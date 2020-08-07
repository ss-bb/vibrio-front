<template>
    <v-theme-provider dark>
        <base-section id="contact-us" class="secondary" space="36">
            <v-row class="ma-0 d-flex flex-column" align="center" justify="center">
                <v-responsive class="px-4 mx-6" max-width="600" width="100%">
                    <v-text-field label="Newsletter - renseignez votre mail"></v-text-field>
                </v-responsive>

                <div
                    class="mt-3 d-flex flex-row justify-space-between align-center newsletter__div"
                >
                    <base-img
                        :src="require('@/assets/img/fb_vibrio.svg')"
                        contain
                        width="50px"
                        height="50px"
                    />
                    <base-img
                        :src="require('@/assets/img/insta_vibrio.svg')"
                        contain
                        width="50px"
                        height="50px"
                    />
                    <base-img
                        :src="require('@/assets/img/twitter_vibrio.svg')"
                        contain
                        width="50px"
                        height="50px"
                    />
                    <base-img
                        :src="require('@/assets/img/linkedin_vibrio.svg')"
                        contain
                        width="50px"
                        height="50px"
                    />

                    <v-btn class="ml-n1" height="40" outlined style="margin-top: -7px;">Inscription</v-btn>
                </div>
            </v-row>
        </base-section>
    </v-theme-provider>
</template>

<script>
export default {
    name: "SectionNewsletterAlt"
};
</script>

<style lang="scss" scoped>
.newsletter__div {
    width: 600px;
}
</style>
