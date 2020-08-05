<script>
// Extensions
import View from "@/views/View";

// Mixins
import LoadSections from "@/mixins/load-sections";

export default {
    name: "404",

    metaInfo: { title: "Oops! No Page Found" },

    extends: View,

    mixins: [LoadSections(["404", "newsletter", "info-alt"])],

    props: {
        id: {
            type: String,
            default: "about"
        }
    }
};
</script>
