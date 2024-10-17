<script setup>
import EventCard from '@/components/EventCard.vue'
import { ref } from 'vue'

const events = ref([
  {
  id: 5228101,
  category: 'animal welfare',
  title: 'Cat Adoption Day',
  description: 'Find your new feline friend at this event.',
  location: 'Meow Town',
  date: 'January 28, 2022',
  time: '12:00',
  petsAllowed: true,
  organisazier: 'Kat Laydee'
},
{
  id: 5948101,
  category: 'animal welfare',
  title: 'Communety Gardening',
  description: 'Find your new feline friend at this event.',
  location: 'Meow Town',
  date: 'January 28, 2022',
  time: '12:00',
  petsAllowed: true,
  organisazier: 'Kat Laydee'
},
{
  id: 5928501,
  category: 'animal welfare',
  title: 'Beach cleanup',
  description: 'Find your new feline friend at this event.',
  location: 'Meow Town',
  date: 'January 28, 2022',
  time: '12:00',
  petsAllowed: true,
  organisazier: 'Kat Laydee'
}])
</script>

<template>
  <h1>Events for Good</h1>
  <div class="events"> 
    <EventCard v-for="event in events" :key="event.id" :event="event"/>
  </div>
</template>

<style scoped>
.events{
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>