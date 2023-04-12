<script>
export default {
  setup(props) {
    // ...
    onMounted(() => {
      console.log("title: " + props.title);
    });
    // ...
  },
};
</script>