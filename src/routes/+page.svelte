
<script>
  import { Alert } from 'flowbite-svelte';
    import { MailBoxOutline } from 'flowbite-svelte-icons';


</script>

<div class="grid grid-cols-1 gap-2 md:grid-cols-2 items-start">
  <div class="bg-gray-100 px-8 py-2 rounded-xl md:col-span-2">
    <h2 class="text-2xl md:text-3xl font-extrabold dark:text-white my-5">Willkommen bei den Thierberger Schützen!</h2>
    <p class="my-3">In unserer Gilde und Kompanie verbinden wir die Werte des historischen Schützenwesens mit modernem Training und sportlichem Ehrgeiz. Ob beim regelmäßigen Schießtraining, bei Wettkämpfen oder bei geselligen Zusammenkünften – bei uns stehen Kameradschaft, Heimatverbundenheit und die Förderung der Schützentradition im Mittelpunkt.</p>
    <p class="my-3">Neben dem Schießsport engagieren wir uns aktiv im gesellschaftlichen Leben der Region. Als Veranstalter des Maibaumfests pflegen wir ein jahrhundertealtes Brauchtum und sorgen für ein geselliges Miteinander. Zudem sind wir stolze Standbetreiber beim Zeller Fest, wo wir die Tradition der Schützen mit kulinarischen Spezialitäten und guter Stimmung erlebbar machen. Wir laden alle ein, Teil unserer Gemeinschaft zu werden – sei es als aktiver Schütze, Unterstützer oder Besucher unserer Veranstaltungen!</p>
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

  iframe{
    max-height: 100vh; 
    @media only screen and (max-width: 47.9rem){max-height:70vh}
  }

</style>
  
