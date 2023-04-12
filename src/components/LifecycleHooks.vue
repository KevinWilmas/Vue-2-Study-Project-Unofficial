<script>
import { reactive, onMounted } from "vue";
export default {
  props: {
    title: String,
  },
  setup() {
    // ..
    onMounted(() => {
      console.log("component mounted");
    });
    // ...
  },
};
</script>