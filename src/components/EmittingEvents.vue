<script>
export default {
  methods: {
    login() {
      this.$emit("login", {
        username: this.username,
        password: this.password,
      });
    },
  },
};
</script>