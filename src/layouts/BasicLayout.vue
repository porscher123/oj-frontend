<template>
  <div id="basicLayout">
    <a-layout style="height: 400px;">
      <a-layout-header class="header">
        <GlobalHeader></GlobalHeader>
      </a-layout-header>

     
      <a-layout-content class="content">
        <router-view/>
      </a-layout-content>
        

      <a-layout-footer class="footer">
        super OJ by xinchao wang
      </a-layout-footer>
    </a-layout>
  </div>
</template>
<script>
  import GlobalHeader from '@/components/GlobalHeader.vue'
  export default {
    components: {
      GlobalHeader
    }
  }
</script>

<style scoped>

#basicLayout .header {
  background: red;
  margin-bottom: 16px;
}

#basicLayout .content {
  background: linear-gradient(to right, #edf, #dff);
  margin-bottom: 16px;
}

#basicLayout .footer {
  background: blanchedalmond;
  padding: 16px;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  text-align: center;
}

</style>


