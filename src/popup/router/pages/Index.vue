<template>

<div style="width:700px">
  <p>fdsgfddfgdgdgdgdfgHello world!{{animatedNumber}} fdsvfg</p>
      <dx-button :text='text'/>
      <QueriesGrid/>
</div>

</template>

<script>
import DxButton from 'devextreme-vue/button';
import QueriesGrid from './QueriesGrid';
export default {
 mounted() {
  },
  data() {
    return {
      text: "click",
      animatedNumber: this.$store.getters.foo,
      queries:{
        name:"default",
        selectors:[
          "page"
        ]
      }
    };
  },
  components: {
    DxButton,
    QueriesGrid
  }
};
</script>

<style lang="scss" scoped>
</style>
