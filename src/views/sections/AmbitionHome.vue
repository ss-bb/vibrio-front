<template>
    <base-section id="ambition-home" class="secondary d-flex">
        <v-row align="center">
            <v-col cols="12" offset-md="1" md="4">
                <div>
                    <base-heading
                        class="white--text mb-12"
                        size="display-1"
                        title="Notre ambition"
                    />
                    <p
                        class="grey--text"
                    >Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
                    <p
                        class="grey--text"
                    >Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt.</p>
                    <p
                        class="grey--text"
                    >Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur?</p>
                </div>
            </v-col>
            <v-col cols="12" md="6" offset-md="1">
                <base-img
                    class="ambitionhome__img"
                    :src="require('@/assets/agence-home.jpg')"
                    contain
                    width="100%"
                    max-height="600px"
                />
            </v-col>
        </v-row>
    </base-section>
</template>

<script>
export default {
    name: "SectionAmbitionHome",

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

<style lang="scss" scoped>
.ambitionhome__img {
}
</style>
