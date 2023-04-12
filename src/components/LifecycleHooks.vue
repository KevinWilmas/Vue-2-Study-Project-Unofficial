<script>
export default {
  props: {
    title: String,
  },
  data() {
    return {
      username: "",
      password: "",
    };
  },
  mounted() {
    console.log("component mounted");
  },
  methods: {
    login() {
      // login method
    },
  },
};
</script>