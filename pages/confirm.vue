<script setup>
definePageMeta({
  middleware: "redirect",
});
</script>

<template>
  <ClientOnly>
    <FeedbackSection />
    <template #fallback>
      <div class="flex w-full justify-center items-center">
        <Skeleton class="h-[700px] w-full rounded-xl mt-10" />
      </div>
    </template>
  </ClientOnly>
</template>
