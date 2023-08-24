<template>
  <article class="post-container hover:transform hover:scale-105 transition-transform duration-300">
    <h2 class="content-date">
      <a href="#2022-06-23" class="date-link hover:underline">{{ content.date }}</a>
    </h2>
    <div class="content-block">
      <div class="feed-border"></div>
      <div class="feed-dot"></div>
      <badge
        :label="`v ${content.version}`"
        class="absolute -top-6 right-0 md:static mb-4"
      />
      <h1 v-if="content.title" class="title">
        {{ content.title }}
      </h1>
      <ContentRenderer :value="content" class="document" />
      <Authors v-if="content.authors" :authors="content.authors" />
    </div>
  </article>
</template>

<style>
.post-container {
  @apply md:flex mt-8;
}

.feed-dot {
  @apply absolute -top-[1.0625rem] -left-1 h-[0.5625rem] w-[0.5625rem] rounded-full border-2 border-slate-300 bg-white md:top-[0.4375rem];
}

.feed-border {
  @apply absolute -bottom-2 left-0 w-px bg-slate-200 -top-3 md:top-2.5;
}

.content-date {
  @apply pl-7 text-xs sm:text-sm leading-6 text-slate-500 font-bold md:w-1/4 md:pl-0 md:pr-12 md:text-right;
}

.date-link {
  @apply transition-colors duration-300;
  @apply hover:text-teal-500;
}

.content-block {
  @apply relative pt-2 pl-7 md:w-3/4 md:pt-0 md:pl-12 pb-16;
}

.title {
  @apply text-teal-500 text-xl sm:text-3xl font-bold mb-4;
}

.document {
  @apply max-w-none prose-h3:mb-4 prose-h3:text-base prose-h3:leading-6 prose-sm prose prose-pre:text-base prose-slate prose-a:font-semibold prose-a:text-primary hover:prose-a:text-sky-600;
}
</style>
