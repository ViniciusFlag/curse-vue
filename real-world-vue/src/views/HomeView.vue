<template>
  <div class="events">
    <h1>Events for Good</h1>
    <EventCard v-for="event in events" :key="event.id" :event="event" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: "HomeView",
  components: {
    EventCard,
  },

  data() {
    return {
      events: [
        {
          id: 1234,
          category: "food & drink",
          title: "Community Gardening",
          description: "Learn how to grow your own organic vegetables.",
          location: "Green Valley",
          date: "March 12, 2022",
          time: "09:00",
          petsAllowed: true,
          organize: "Flora Green",
        },
        {
          id: 1235,
          category: "food & drink",
          title: "Community Gardening",
          description: "Learn how to grow your own organic vegetables.",
          location: "Green Valley",
          date: "March 12, 2022",
          time: "09:00",
          petsAllowed: true,
          organize: "Flora Green",
        },
        {
          id: 1236,
          category: "sustainability",
          title: "Beach Clean-up",
          description: "Help us keep our coastline beautiful and plastic-free.",
          location: "Sandy Shores",
          date: "April 22, 2022",
          time: "08:30",
          petsAllowed: false,
          organize: "Eco Watch",
        },
        {
          id: 1237,
          category: "animal welfare",
          title: "Puppy Training Workshop",
          description: "Basic obedience and socialization for your new pup.",
          location: "Bark Park",
          date: "May 15, 2022",
          time: "14:00",
          petsAllowed: true,
          organize: "Doggo Academy",
        },
        {
          id: 1238,
          category: "education",
          title: "Intro to Coding",
          description: "A beginner-friendly workshop on JavaScript basics.",
          location: "Tech Hub",
          date: "June 10, 2022",
          time: "18:30",
          petsAllowed: false,
          organize: "Code Masters",
        },
        {
          id: 1239,
          category: "health",
          title: "Yoga in the Park",
          description: "Relaxing morning flow for all skill levels.",
          location: "Central Park",
          date: "July 05, 2022",
          time: "07:00",
          petsAllowed: true,
          organize: "Zen Vibes",
        },
      ],
    };
  },
};
</script>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
