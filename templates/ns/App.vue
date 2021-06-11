<template>
  <Page actionBarHidden="true">

    <!-- <ActionBar title="OneFocus" android:flat="true"/> -->

    <TabView android:tabBackgroundColor="#53ba82"
              android:tabTextColor="#c4ffdf"
              android:selectedTabTextColor="#ffffff"
              androidSelectedTabHighlightColor="#ffffff"
              androidTabsPosition="bottom"
              selectedIndex="1">

      <!-- <TabViewItem class="fas" title.decode="Home &#xf015;"> -->
      <TabViewItem title="Component 1">
        <GridLayout columns="*" rows="*">
          <Component1/>
        </GridLayout>
      </TabViewItem>

      <!-- <TabViewItem class="fas" title.decode="Tasks &#xf0ae;"> -->
      <TabViewItem title="Component 2">
        <GridLayout columns="*" rows="*">
          <Component2/>
        </GridLayout>
      </TabViewItem>



    </TabView>

  </Page>
</template>

<script>
import Component1 from "./Component1.vue";
import Component2 from "./Component2.vue";

export default {
  components: {
    Component1,
    Component2,
  }
};

</script>

<style scoped>
ActionBar {
  background-color: #53ba82;
  color: #ffffff;
}
</style>
