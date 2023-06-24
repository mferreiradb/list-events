<script setup>
import EventCard from '@/components/EventCard.vue';
import { ref } from 'vue';

const events = ref([
{
  id: 1,
  category: 'Animal',
  title: 'Cat adoption day',
  description: 'Find you a new feline friend at this event.',
  location: 'Meow town',
  date: 'January 28, 2023',
  time: '22:00',
  petAllowed: true,
  organizer: 'Kat Laydee '
},
{
  id: 2,
  category: 'Animal',
  title: 'Monkey adoption day',
  description: 'Find you a new monkey friend at this event.',
  location: 'HUHAHAHA town',
  date: 'January 29, 2023',
  time: '22:00',
  petAllowed: true,
  organizer: 'Monk Laydee '
},
{
  id: 3,
  category: 'Animal',
  title: 'Dog adoption day',
  description: 'Find you a new dog friend at this event.',
  location: 'Doo town',
  date: 'January 30, 2023',
  time: '22:00',
  petAllowed: true,
  organizer: 'Scoob Laydee '
}
])

</script>

<template>
  <h1>Events For Good</h1>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event"/>
  </div>
</template>

<style scoped>
  .events {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
</style>