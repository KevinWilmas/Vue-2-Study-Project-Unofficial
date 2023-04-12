<script>
import { reactive } from "vue";
export default {
  props: {
    title: String,
  },
  setup() {
    const state = reactive({
      username: "",
      password: "",
    });
    return { state };
  },
};
</script>