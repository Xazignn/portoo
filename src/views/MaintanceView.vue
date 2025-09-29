<template>
  <div class="flex items-center justify-center min-h-screen bg-gradient-to-br p-6">
    <div class="text-center text-white max-w-lg fade-zoom-up">
      <!-- Icon / Illustration -->
      <div class="flex justify-center mb-6">
        <img src="https://cdn-icons-png.flaticon.com/512/864/864685.png" alt="Maintenance" class="w-28 md:w-36 animate-bounce filter invert" />
      </div>

      <!-- Title -->
      <h1 class="text-2xl md:text-4xl font-bold bg-clip-text text-transparent bg-gradient-to-r from-amber-300 to-yellow-500">
        We’ll Be Back Soon!
      </h1>

      <!-- Subtitle -->
      <p class="mt-4 text-slate-300 text-sm md:text-base leading-relaxed">
        Our website is currently undergoing scheduled maintenance.  
        We’re working hard to bring you a better experience.  
        Please check back again later.
      </p>

      <!-- Divider -->
      <div class="h-[1px] mt-7 mb-7 w-24 mx-auto bg-amber-200"></div>

      <!-- Contact Info -->
      <p class="text-xs md:text-sm text-slate-400">
        Need immediate assistance?  
        <a href="mailto:support@example.com" class="text-amber-300 hover:underline">Contact Support</a>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "MaintenancePage"
}
</script>

<style scoped>
@keyframes fadeZoomUp {
  0% {
    opacity: 0;
    transform: translateY(40px) scale(0.9);
  }
  100% {
    opacity: 1;
    transform: translateY(0) scale(1);
  }
}
.fade-zoom-up {
  animation: fadeZoomUp 1s ease-in-out forwards;
}
</style>
