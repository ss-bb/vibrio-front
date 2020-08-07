<template>
    <v-theme-provider dark>
        <base-section id="info-alt" class="secondary">
            <v-responsive class="mx-auto" max-width="1400">
                <v-container fluid>
                    <v-row>
                        <v-col cols="12" md="3">
                            <span class="white--text">pas compris le design</span>
                        </v-col>

                        <v-col cols="12" md="3">
                            <base-img
                                :src="require('@/assets/img/logo.svg')"
                                contain
                                width="200px"
                                height="200px"
                            />
                        </v-col>

                        <v-col class="d-flex flex-column white--text" cols="12" md="2">
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
                        </v-col>

                        <v-col class="d-flex justify-space-between white--text" cols="12" md="4">
                            <div class="d-flex flex-column white--text">
                                <p v-for="(name, i) in items" :key="i">{{ name }}</p>
                            </div>
                            <div class="d-flex flex-column white--text">
                                <p v-for="(name, j) in mentions" :key="j">{{ name }}</p>
                            </div>
                        </v-col>
                    </v-row>
                </v-container>
            </v-responsive>
        </base-section>
    </v-theme-provider>
</template>

<script>
export default {
    name: "SectionBusinessInfo",

    components: {
        InfoFeatures: () => import("@/components/InfoFeatures"),
        Instagram: () => import("@/components/Instagram")
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
            "Evenements"
        ],
        mentions: [
            "Legal",
            "Mentions Légales / CGU",
            "Politique de confidentialité",
            "Cookies",
            "Crédits"
        ]
    })
};
</script>

<style lang="sass">
#info-alt a
    text-decoration: none
</style>
