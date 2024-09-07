<script setup>
  import { RouterLink } from 'vue-router';
  import Card from './Card.vue';
</script>


<template>
    <section class="py-4">
      <div class="container-xl lg:container m-auto">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-4 p-4 rounded-lg">
          <Card>
            <h2 class="text-2xl font-bold">For Pirates</h2>
            <p class="mt-2 mb-4">
              Browse our Ships and start your career today
            </p>
            <RouterLink to="/Ships" class="inline-block bg-black text-white rounded-lg px-4 py-2 hover:bg-gray-700">
              Browse Ships
            </RouterLink>
          </Card>
          <Card bg="bg-green-100">
            <h2 class="text-2xl font-bold">For Captains</h2>
            <p class="mt-2 mb-4">
              List your job to find the perfect Pirates for the role in your crew
            </p>
            <RouterLink to="/ships/add" class="inline-block bg-green-500 text-white rounded-lg px-4 py-2 hover:bg-green-600">
              Add Ship
            </RouterLink>
          </Card>
        </div>
      </div>
    </section>
</template>