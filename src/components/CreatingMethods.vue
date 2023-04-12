<script>
export default {
  props: {
    title: String,
  },
  setup() {
    const state = reactive({
      username: "",
      password: "",
    });
    const login = () => {
      // login method
    };
    return {
      login,
      state,
    };
  },
};
</script>