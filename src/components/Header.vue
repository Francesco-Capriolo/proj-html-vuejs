<template>
  <section class="container-fluid">
    <TopHeader />
    <SearchHeader />
    <IconsHeader />
  </section>
</template>

<script>
import TopHeader from "./TopHeader.vue";
import SearchHeader from "./SearchHeader.vue";
import IconsHeader from "./IconsHeader.vue";

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