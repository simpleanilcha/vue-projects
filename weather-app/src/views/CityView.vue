<template>
  <div>
    <Suspense>
      <AsyncCityView />
      <template #fallback>
        <!-- <p class="text-white text-center py-10">Loading...</p> -->
        <CityViewSkeleton />
      </template>
    </Suspense>
  </div>
</template>

<script setup>
import AsyncCityView from '../components/AsyncCityView.vue';
import CityViewSkeleton from '../components/CityViewSkeleton.vue';

</script>
