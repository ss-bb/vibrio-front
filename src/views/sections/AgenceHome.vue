<template>
    <base-section id="agence-home" class="secondary">
        <v-container class="fill-height px-4 py-12">
            <v-responsive class="d-flex align-center" height="100%" max-width="1000" width="100%">
                <base-heading
                    class="white--text ml-12"
                    size="display-1"
                    title="Nous sommes agence événementiel,"
                />
                <base-heading
                    class="white--text ml-12"
                    size="display-1"
                    title="et tellement plus."
                />
            </v-responsive>
        </v-container>
        <v-row align="center" class="px-12">
            <v-col cols="12" md="7">
                <base-img :src="require('@/assets/logo.svg')" contain width="100%" height="800px" />
            </v-col>

            <v-col cols="12" md="4" class="px-12">
                <p
                    class="grey--text"
                >Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
                <p
                    class="grey--text"
                >Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt.</p>
                <p
                    class="grey--text"
                >Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur?</p>
            </v-col>
        </v-row>
    </base-section>
</template>

<script>
export default {
    name: "SectionAgenceHome",

    data: () => ({
        features: [
            ["Components", 23, "40+"],
            ["Example Pages", 3, 10],
            ["Bugfixes and Issues", true, true],
            ["Vue CLI Support", true, true],
            ["News, Project, and Pricing Pages", false, true],
            ["6 Months Free Updates", false, true],
            ["Price", "Free", "$60"]
        ]
    })
};
</script>
