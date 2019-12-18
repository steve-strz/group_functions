<template>
  <Page actionBarHidden="true">
    <StackLayout verticalAlignment="center" horizontalAlignment="center">
      <button
        text="Go to group"
        fontSize="20"
        backgroundColor="#53ba82"
        width="50%"
        color="white"
        @tap="goto_group"
      />
    </StackLayout>
  </Page>
</template>

<script >
import Group from "../views/Group";
import SidebarMenuGroup from "./SidebarMenuGroup";

export default {
  data() {
    return {};
  },
  methods: {
    goto_group() {
      this.$navigateTo(Group, {
        transition: "slide",
        duration: 200
      });
    }
  },
  components: {
    Group,
    SidebarMenuGroup
  }
};
</script>

<style scoped>
</style>
