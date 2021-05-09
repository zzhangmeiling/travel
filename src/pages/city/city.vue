<template>
  <div>
    <city-header />
    <city-search />
  </div>
</template>
<script>
import CityHeader from "./components/header";
import CitySearch from "./components/search";
export default {
  name: "City",
  components: {
    "city-header": CityHeader,
    "city-search": CitySearch,
  },
  data() {
    return {};
  },
};
</script>
<style scoped>
</style>