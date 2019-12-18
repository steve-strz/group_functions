<template>
  <Page actionBarHidden="true">
    <StackLayout orientation="horizontal" verticalAlignment="center">
      <GridLayout columns="*" rows="*" verticalAlignment="center" horizontalAlignment="center">
        <Label text="This is my group" column="0" row="0" fontSize="30" />
      </GridLayout>
      <StackLayout
        verticalAlignment="center"
        horizontalAlignment="center"
        v-if="showSidebar"
        marginRight="-20"
      >
        <SidebarMenuGroup />
      </StackLayout>
    </StackLayout>
  </Page>
</template>

<script >
import SidebarMenuGroup from "../components/SidebarMenuGroup.vue";

export default {
  name: "group",
  data() {
    return {
      showSidebar: true
    };
  },
  methods: {},
  components: {
    SidebarMenuGroup
  }
};
</script>

<style scoped>
</style>
