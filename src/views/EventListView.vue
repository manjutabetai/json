<script setup>
import EventCard from '@/components/EventCard.vue'
import { ref } from 'vue'

const events = ref([
  {
    id: 12344,
    category: 'animal welfare-1',
    title: 'Cat Adoption Day',
    description: 'Find your new feline friend at this event.',
    location: 'Meow Town',
    date: 'January 28,2022',
    time: '13:00',
    petsAllowed: true,
    organizer: 'Kat Laydee'
  },
  {
    id: 12332,
    category: 'animal welfare-2',
    title: 'Cat Adoption Day',
    description: 'Find your new feline friend at this event.',
    location: 'Meow Town',
    date: 'January 28,2022',
    time: '13:00',
    petsAllowed: true,
    organizer: 'Kat Laydee'
  },
  {
    id: 124,
    category: 'animal welfare-3',
    title: 'Cat Adoption Day',
    description: 'Find your new feline friend at this event.',
    location: 'Meow Town',
    date: 'January 28,2022',
    time: '13:00',
    petsAllowed: true,
    organizer: 'Kat Laydee'
  }
])
</script>

<template>
  <div class="events">
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
