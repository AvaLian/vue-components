<template>
  <layout>
    <x-header slot="header">
      <div slot="title">Divider</div>
    </x-header>
    <x-body slot="body">
      <div style="background:#fff;margin:15px 0;padding:1px 10px;line-height:40px;">
        标题
        <divider></divider>
        内容....
      </div>
    </x-body>
  </layout>
</template>

<script>
import {
  Layout,
  XHeader,
  XBody,
  Group,
  Divider
} from 'components'
export default {
  components: {
    Layout,
    XHeader,
    XBody,
    Group,
    Divider
  },
  methods: {
    changeHandler (value) {
      this.value = value
    }
  },
  data () {
    return {
      value: '',
      options: [
        {
          value: '1',
          label: '篮球'
        },
        {
          value: '2',
          label: '羽毛球'
        },
        {
          value: '3',
          label: '乒乓球'
        },
        {
          value: '4',
          label: '高尔夫'
        }
      ]
    }
  }
}
</script>

<style lang="scss">

</style>
