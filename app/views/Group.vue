<template>
  <Page actionBarHidden="true">
    <GridLayout columns="*, *" rows="*, *" verticalAlignment="center" horizontalAlignment="center">
      <Label text="This is my group" column="0" row="0" fontSize="30" />
      <SidebarMenuGroup column="1" row="1" />
    </GridLayout>
  </Page>
</template>

<script >
import SidebarMenuGroup from "../components/SidebarMenuGroup.vue";

export default {
  name: "group",
  data() {
    return {};
  },
  methods: {},
  components: {
    SidebarMenuGroup
  }
};
</script>

<style scoped>
</style>
