
<script>
  import { Alert } from 'flowbite-svelte';


</script>

<div class="grid grid-cols-1 gap-2 md:grid-cols-2 items-start">
  <div class="bg-gray-100 px-8 py-2 rounded-xl md:col-span-2">
    <h2 class="text-2xl md:text-3xl font-extrabold dark:text-white my-5">Willkommen bei den Thierberger Schützen!</h2>
    <p class="my-3">Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</p>

  </div>
  

  <div class="bg-gray-100 px-8 py-2 rounded-xl">
    <h3 class="text-2xl md:text-3xl font-extrabold dark:text-white my-3">News</h3>
    
    <iframe title="Social Media Posts" src="https://www.juicer.io/api/feeds/thierberger-schutzen/iframe" frameborder="0" width="100%" height="800" style="display:block;"></iframe>
  </div>
  
  <div class="bg-gray-100 px-8 py-2 rounded-xl">
    <h3 class="text-2xl md:text-3xl  font-extrabold dark:text-white my-3">Termine</h3>
    <iframe title="Terminübersicht" src="https://calendar.google.com/calendar/embed?height=600&wkst=2&ctz=Europe%2FVienna&showPrint=0&showTitle=0&showTz=0&mode=AGENDA&showNav=0&showTabs=0&showCalendars=0&showDate=0&title=Termine&src=d2VibWFuYWdtZW50LnRoaWVyYmVyZ0BnbWFpbC5jb20" width="100%" height="600" frameborder="0" scrolling="no"></iframe>
  
  </div>

</div>


<style>
.referral{
  display: none;
}

</style>
  
