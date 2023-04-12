<script>
export default {
  setup(props, { emit }) {
    // ...
    const login = () => {
      emit("login", {
        username: state.username,
        password: state.password,
      });
    };
    // ...
  },
};
</script>