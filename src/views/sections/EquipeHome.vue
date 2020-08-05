<template>
    <base-section id="ambition-home" class="secondary d-flex">
        <v-row align="center">
            <v-col cols="12" class="d-flex justify-center">
                <div class="module mx-12">
                    <p class="stripe mb-0"></p>
                </div>
            </v-col>
            <v-col cols="12" class="d-flex justify-center my-6">
                <base-heading class="white--text ml-12" size="display-1" title="Notre équipe" />
            </v-col>
            <v-col cols="3" class="d-flex flex-column justify-center align-center">
                <v-avatar size="130">
                    <base-img :src="require('@/assets/img/equipe1.jpg')" />
                </v-avatar>
                <base-subheading class="white--text mt-3 mb-0" title="XYZ yolo" />
                <base-subheading class="grey--text mt-0" title="CHEF chef" />
            </v-col>
            <v-col cols="3" class="d-flex flex-column justify-center align-center">
                <v-avatar size="130">
                    <base-img :src="require('@/assets/img/equipe2.jpg')" />
                </v-avatar>
                <base-subheading class="white--text mt-3 mb-0" title="LAUTRE la" />
                <base-subheading class="grey--text mt-0" title="il bosse bien" />
            </v-col>
            <v-col cols="3" class="d-flex flex-column justify-center align-center">
                <v-avatar size="130">
                    <base-img :src="require('@/assets/img/equipe3.jpg')" />
                </v-avatar>
                <base-subheading class="white--text mt-3 mb-0" title="ABC def" />
                <base-subheading class="grey--text mt-0" title="drole de nom" />
            </v-col>
            <v-col cols="3" class="d-flex flex-column justify-center align-center">
                <v-avatar size="130">
                    <base-img :src="require('@/assets/img/equipe4.jpg')" />
                </v-avatar>
                <base-subheading class="white--text mt-3 mb-0" title="PAS moi" />
                <base-subheading class="grey--text mt-0" title="pas taper" />
            </v-col>
            <v-col cols="3" class="d-flex flex-column justify-center align-center">
                <v-avatar size="130">
                    <base-img :src="require('@/assets/img/equipe5.jpg')" />
                </v-avatar>
                <base-subheading class="white--text mt-3 mb-0" title="MARTIN pierre" />
                <base-subheading class="grey--text mt-0" title="DEV front" />
            </v-col>
            <v-col cols="3" class="d-flex flex-column justify-center align-center">
                <v-avatar size="130">
                    <base-img :src="require('@/assets/img/equipe2.jpg')" />
                </v-avatar>
                <base-subheading
                    class="white--text text-center mt-3 mb-0"
                    title="UN NOM BEAUCOUP TROP LONG jean-françois"
                />
                <base-subheading class="grey--text mt-0" title="voila" />
            </v-col>
            <v-col cols="12" class="d-flex justify-center">
                <div class="module mx-12">
                    <p class="stripe mb-0"></p>
                </div>
            </v-col>
        </v-row>
    </base-section>
</template>

<script>
export default {
    name: "SectionEquipeHome"
};
</script>

<style lang="scss">
.module {
    background: white;
    border: 1px solid #ccc;
    width: 80%;
}

.stripe {
    height: 20px;
    color: black;
    background: repeating-linear-gradient(
            45deg,
            transparent,
            transparent 10px,
            #eee 10px,
            #111 20px
        ),
        linear-gradient(to bottom, #eee, #000);
}
</style>
