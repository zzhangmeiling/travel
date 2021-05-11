<template>
  <div>
    <city-header />
    <city-search />
    <city-list/>
  </div>
</template>
<script>
import CityHeader from "./components/header";
import CitySearch from "./components/search";
import CityList from "./components/list";
export default {
  name: "City",
  components: {
    "city-header": CityHeader,
    "city-search": CitySearch,
    "city-list":CityList
  },
  data() {
    return {};
  },
};
</script>
<style scoped>
</style>