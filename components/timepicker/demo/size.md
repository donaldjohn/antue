---
order: 2
title:
  zh-CN: 三种大小
  en-US: Three Sizes
---

## zh-CN

三种大小的输入框，大的用在表单中，中的为默认。

## en-US

The input box comes in three sizes. large is used in the form, while the medium size is the default.

```` html
<template>
  <div>
    <time-picker v-model="time1" size="large"/>
    <time-picker v-model="time2"/>
    <time-picker v-model="time3" size="small"/>
  </div>
</template>

<script>
import TimePicker from '@/timepicker'
import moment from 'moment'

export default {
  components: {
    TimePicker
  },
  data () {
    return {
      time1: moment('12:08:23', 'HH:mm:ss'),
      time2: moment('12:08:23', 'HH:mm:ss'),
      time3: moment('12:08:23', 'HH:mm:ss')
    }
  }
}
</script>

````
