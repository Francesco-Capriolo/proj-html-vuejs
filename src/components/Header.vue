<template>
  <section>
    <TopHeader />
    <SearchHeader />
    <IconsHeader />
  </section>
</template>

<script>
import TopHeader from "./headerComponents/TopHeader.vue";
import SearchHeader from "./headerComponents/SearchHeader.vue";
import IconsHeader from "./headerComponents/IconsHeader.vue";

export default {
  name: "IndexHeader",
  components: {
    TopHeader,
    SearchHeader,
    IconsHeader,
  },
};
</script>

<style lang="scss">
.d-flex {
  padding: 0;
}

.top-search {
  margin: 0 0.3rem;
}
i {
  margin: 0 0.3rem;
}
</style>