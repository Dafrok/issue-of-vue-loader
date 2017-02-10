<template>
<div>
<h2>GoodCase(Correctly mounted):</h2>
<good-case />
<h2>BadCase(can't be mounted and cause a warning):</h2>
<bad-case />
</div>
</template>

<script>
import GoodCase from './components/good-case.js'
import BadCase from './components/bad-case.js'
export default {
  components: {
    GoodCase,
    BadCase
  }
}
</script>