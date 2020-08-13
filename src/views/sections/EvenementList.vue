<template>
    <base-section id="evenement-liste">
        <base-section-heading title="Nos événements"></base-section-heading>

        <v-container>
            <v-row>
                <v-col v-for="(evenement, i) in evenements" :key="i" cols="12" md="4">
                    <base-avatar-card v-bind="evenement" align="left" horizontal>des trucs de fou</base-avatar-card>
                </v-col>
            </v-row>
        </v-container>
    </base-section>
</template>

<script>
export default {
    name: "SectionEvenementList",

    data: () => ({
        features: [
            {
                title: "Basic",
                icon: "mdi-fountain-pen-tip"
            },
            {
                title: "Boom BOOM",
                icon: "mdi-cellphone"
            },
            {
                color: "Basic",
                dark: true,
                title: "Easily Customizable",
                icon: "mdi-pencil-box-outline"
            },
            {
                title: "Basic",
                icon: "mdi-image-size-select-actual"
            },
            {
                title: "Basic",
                icon: "mdi-ice-pop"
            },
            {
                title: "Basic",
                icon: "mdi-help-circle-outline"
            }
        ]
    })
};
</script>
