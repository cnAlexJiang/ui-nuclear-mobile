<template>
  <WingBlank>
    <h3>基本</h3>
    <p>Without text</p>
    <ActivityIndicator></ActivityIndicator>
    <p>With text</p>
    <ActivityIndicator text="loading..." size="small"></ActivityIndicator>
    <p>With large size and customized text style</p>
    <ActivityIndicator text="loading..." size="large" align="vertical" style="font-size: 16px;color: #000"></ActivityIndicator>
  </WingBlank>
</template>

<script>
  import WingBlank from '@/components/WingBlank'
  import Button from '@/components/Button'
  import WhiteSpace from '@/components/WhiteSpace'
  import ActionSheet from '@/components/ActionSheet'
  import ActivityIndicator from '@/components/ActivityIndicator'

  export default{
    components: {
      WingBlank,
      ActionSheet,
      Button,
      WhiteSpace,
      ActivityIndicator
    },
    data () {
      return {}
    }
  }
</script>

<style>
p {
  color: #888;
}
</style>

