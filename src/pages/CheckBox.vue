<template>
  <div>
    <WingBlank>
      <h3>基本</h3>
    </WingBlank>
    <List renderHeader="CheckboxItem demo">
      <CheckboxItem Title="Barcelona" defaultChecked></CheckboxItem>
      <CheckboxItem Title="Stuttgart" ></CheckboxItem>
      <CheckboxItem Title="Paris" extra="extra content"></CheckboxItem>
      <CheckboxItem Title="Liverpool" disabled defaultChecked subtitle="Disable options"></CheckboxItem>
    </List>
    <AgreeItem>Agree 
      <a @click="onClick">agreement</a></AgreeItem>
  </div>
</template>

<script>
  import Button from '@/components/Button'
  import { Checkbox, CheckboxItem, AgreeItem } from '@/components/Checkbox'
  import WingBlank from '@/components/WingBlank'
  import WhiteSpace from '@/components/WhiteSpace'
  import { Flex, FlexItem } from '@/components/Flex'
  import { List, ListItem, ListItemBrief } from '@/components/List'

  export default {
    components: {
      WingBlank,
      WhiteSpace,
      Checkbox,
      List,
      ListItem,
      ListItemBrief,
      CheckboxItem,
      Button,
      AgreeItem,
      Flex,
      FlexItem
    },
    data () {
      return {
        checked: ''
      }
    },
    methods: {
      stuOnChange (value) {
        console.log(value)
      },
      onClick () {
        console.log(234)
      }
    }
  }
</script>

<style>

</style>
