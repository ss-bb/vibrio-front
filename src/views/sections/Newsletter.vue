<template>
    <v-theme-provider dark>
        <base-section id="contact-us" class="secondary" space="36">
            <v-row class="ma-0 d-flex flex-column" align="center" justify="center">
                <v-responsive class="px-4 mx-6" max-width="600" width="100%">
                    <base-text-field hide-details label="Newsletter - renseignez votre mail">
                        <template v-slot:append-outer></template>
                    </base-text-field>
                </v-responsive>
                <div>
                    <span>icone icone</span>
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
