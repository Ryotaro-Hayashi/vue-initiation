<template>
  <div id="root">
    <h1 class="header">Rootコンポーネント</h1>
    <p>これはRootコンポーネントです。</p>
    <foo></foo>
    <bar></bar>
  </div>
</template>

<script>
import Foo from './foo'
import Bar from './bar'

export default {
  components: {
    Foo,
    Bar
  }
}
</script>

<!-- スコープが付いていないグローバルなスタイル定義は、
トップとなるファイルで定義する -->
<style scoped>
#root {
  border: solid 1px blue;
  margin: 4px;
  padding: 4px;
}

.header {
  font-size: 200%;
}

p {
  text-decoration: underline;
}
</style>
