<template>
  <section class="">
    <Navbar />
    <Foot />
    <NuxtPage />
    <Notivue v-slot="item">
      <Notification :item="item" />
    </Notivue>
  </section>
</template>
