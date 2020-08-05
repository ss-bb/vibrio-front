
<script>
// Extensions
import View from "@/views/View";

// Mixins
import LoadSections from "@/mixins/load-sections";

export default {
    name: "Home",

    metaInfo: { title: "Home" },

    extends: View,

    mixins: [
        LoadSections([
            "hero",
            "agence-home",
            "ambition-home",
            "valeur-home",
            "contact-us",
            "equipe-home",
            "newsletter",
            "info"
        ])
    ],

    props: {
        id: {
            type: String,
            default: "home"
        }
    }
};
</script>
