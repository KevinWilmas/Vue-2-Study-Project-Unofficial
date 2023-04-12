<script>
uppercase(string) {
  return string.toUpperCase();
}

export { uppercase };
</script>

<script>
import { uppercase } from "@/filters/strings";

app.config.globalProperties.$filters = {
  uppercase: uppercase
};
</script>

<template>
{{ $filters.uppercase(firstName) }}

</template>



