<template>
  <div class="calendar-year">
    <MonthCard 
      v-for="month in months" 
      :key="month" 
      :month="month" 
    />
  </div>
</template>

<script>
import MonthCard from './MonthCard.vue';

export default {
  name: 'CalendarYear',
  components: {
    MonthCard,
  },
  data: () => ({
    months: 12,
  }),
};
</script>

<style>
.calendar-year {
  display: flex;
  flex-wrap: wrap;
  width: 100%;
};
</style>
