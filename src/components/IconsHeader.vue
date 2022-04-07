<template>
  <div class="row bg-dark align-items-center justify-content-center">
    <div class="d-inline">
      <span class="text-white" v-for="(icon, index) in linksIcons" :key="index">
        <i :class="icon.icon"></i>
        {{ icon.text }}
      </span>
    </div>
  </div>
</template>

<script>
export default {
  name: "IconsHeader",
  data: function () {
    return {
      linksIcons: [
        {
          icon: "fas fa-chart-line",
          text: "Business",
        },
        {
          icon: "fas fa-palette",
          text: "Design",
        },
        {
          icon: "fas fa-cog",
          text: "Development",
        },
        {
          icon: "far fa-smile",
          text: "Lyfestyle",
        },
        {
          icon: "fas fa-print",
          text: "Office Productivity",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.bg-dark {
  height: 6vh;
  span {
    padding: 0 0.5rem;
  }
}
</style>