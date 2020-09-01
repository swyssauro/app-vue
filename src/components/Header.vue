<template>
 <div class="container">
  <b-navbar variant="faded" type="light">
    <b-navbar-brand tag="h1" class="mb-0">
    <b-col class="py-4 mb-2">
      <b-icon 
      icon="exclamation-circle" 
      shift-h="-8" 
      shift-v="-8" 
      class="bg-info">
      </b-icon>
    <b class="logo-quizapp">Quizapp</b>
    </b-col>
    </b-navbar-brand>
    <b-navbar-nav>
      <b-nav-item href="#" disabled>Counter 4/10</b-nav-item>
    </b-navbar-nav>
  </b-navbar>
 </div>
</template>

<style scoped>
.logo-quizapp {
    font-size: 21px;
    font-weight: bolder;
    color: #17a2b8;
}
</style>