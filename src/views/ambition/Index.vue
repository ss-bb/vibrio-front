
<script>
// Extensions
import View from "@/views/View";

// Mixins
import LoadSections from "@/mixins/load-sections";

export default {
    name: "Ambition",

    metaInfo: { title: "Ambition" },

    extends: View,

    mixins: [
        LoadSections([
            "hero",
            "theme-features",
            "features",
            "contact-us",
            "affiliates",
            "social-media",
            "keep-in-touch",
            "newsletter",
            "pro-features",
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
