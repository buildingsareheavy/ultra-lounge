<template>
  <div class="layout">
    <header class="header">
      <GlobalHeader />
    </header>
    <slot />
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
import GlobalHeader from "@/components/global/GlobalHeader";
export default {
  name: "default",
  components: {
    GlobalHeader
  }
};
</script>

<style lang="scss">
.layout {
  max-width: 760px;
  margin: 0 auto;
  padding-right: 1rem;
  padding-left: 1rem;
  min-height: 100vh;
}
.header {
  padding: 0.5em;
}
</style>
