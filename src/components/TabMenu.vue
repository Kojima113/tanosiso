<template>
  <div class="example">
    <div id="tab">
      <TabItem
        v-for="item in list"
        v-bind="item"
        :key="item.id"
        v-model="currentId"
      />
    </div>
  </div>
</template>

<script>
import TabItem from "./TabItem.vue";
export default {
  components: { TabItem },
  data() {
    return {
      currentId: 1,
      list: [
        { id: 1, label: "Tab1" },
        { id: 2, label: "Tab2" },
        { id: 3, label: "Tab3" },
      ],
    };
  },
  computed: {
    current() {
      return this.list.find((el) => el.id === this.currentId) || {};
    },
  },
};
</script>

<style scoped>
.v-leave-active {
    position: absolute;
}
.v-enter {
    transform: translateX(-100%);
}
.v-leave-to {
    transform: translateX(100%);
}
</style>