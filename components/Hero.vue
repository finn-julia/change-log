<template>
  <header class="py-12 px-4 sm:px-6 lg:px-8">
    <div class="relative mx-auto max-w-[37.5rem] pt-20 text-center pb-20">
      <div class="flex items-center justify-center space-x-3">
        <img loading="lazy" src="/logo.png" alt="Logspot" class="h-250 w-250" />
        
      </div>
      
      <p class="mt-4 text-base leading-7 text-slate-700">
        This changelog will represent all changes reflected within Jira Tickets. <br>
        Check out this weekly for announcments and recent changes. 
        <a
          class="text-primary underline"
          href="https://helphopelive.org"
          target="_blank"
          >HHL</a
        >.
      </p>
      <br> 
      <h2
          class="text-xl font-extrabold tracking-tight text-teal-600 sm:text-5xl"
        >
           Change Log
        </h2>
    </div>
  </header>
</template>

<script setup></script>

<style scoped>
.form-input {
  @apply block h-10 w-full rounded-md bg-white pr-3 pl-12 text-slate-900 shadow-md shadow-black/5 ring-1 ring-slate-900/5 placeholder:text-slate-400 focus:outline-none focus:ring-2 focus:ring-primary sm:text-sm sm:leading-6;
}
.form-submit {
  @apply inline-flex justify-center rounded-lg text-sm font-semibold py-2.5 px-4 bg-slate-900 text-white hover:bg-slate-700 ml-4 flex-none;
}
</style>
