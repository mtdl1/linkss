<script setup>
import ContentPerson from './components/ContentPerson.vue';
import ContentPersonSkeleton from './components/ContentPersonSkeleton.vue';
// Change Meta Title


</script>

<template>
  <div>
    <main>
      <Suspense>
        <ContentPerson />
        <template #fallback>
          <ContentPersonSkeleton />
        </template>
      </Suspense>
    </main>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Anta&family=Lexend:wght@100..900&display=swap');

*, *::before, *::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: "Anta", sans-serif;
}

body{
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100dvh;
  background-color: #f1f1f1;
}

main{
  max-width: 620px;
}

/* responsivo */
@media (max-width: 620px){
  main{
    max-width: 95%;
    margin: 0 auto;
  }
}
</style>
