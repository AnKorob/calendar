<template>
  <div :class="{'weekend-day': isItWeekEnd}">
    {{ day }}
  </div>
</template>

<script>
export default {
  name: 'DayCard',
  props: {
    day: Number,
    isItWeekEnd: Boolean,
  },
}
</script>
 
<style>
.weekend-day {
  color: #A00;
};
</style>
