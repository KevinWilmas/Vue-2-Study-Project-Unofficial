<script>
import { reactive, onMounted, computed } from "vue";
export default {
  props: {
    title: String,
  },
  setup() {
    const state = reactive({
      username: "",
      password: "",
      lowerCaseUsername: computed(() => state.username.toLowerCase()),
    });
    // ...
  },
};
</script>