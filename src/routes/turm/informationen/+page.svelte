<script>
    import { Gallery } from 'flowbite-svelte';
    const images = [
      { alt: 'Treppe zur Kapelle', src: '/images/turm/turm1.jpg' },
      { alt: 'Miniatur Nachbau der alten Anlage', src: '/images/turm/turm2.jpg' },
      { alt: 'Blick zum Turm', src: '/images/turm/turm3.jpg' },
      { alt: 'Gipfel Karte', src: '/images/turm/turm5.jpg' },
      { alt: 'Blick zur Kapelle von der Aussichtsplattform', src: '/images/turm/turm8.jpg' },
      { alt: 'Ausstellungsobjekt', src: '/images/turm/turm9.jpg' },
    ];
  </script>
  
  
  <div class="bg-gray-100 px-8 py-2 rounded-xl">
      <h2 class="text-2xl md:text-3xl font-extrabold dark:text-white my-3">Zum Thierberg Turm</h2>
      <p class="my-3">Der Thierberg Turm ist ein beliebtes Ausflugsziel oberhalb von Kufstein und bietet einen atemberaubenden Panoramablick über das Inntal, das Kaisergebirge und die Stadt Kufstein. Öffnungszeiten sind von 09:00 bis 18:00 Uhr.</p>
      <p class="my-3">Im Inneren des Turms befindet sich eine kleine Ausstellung, die sich mit der Geschichte der Burg Thierberg und ihrer Umgebung befasst. Neben historischen Artefakten und Informationen zur mittelalterlichen Bauweise gibt es auch einen Einblick in die religiöse Bedeutung des Ortes.</p>
      <p class="my-3">Der Aufstieg zum Turm ist sowohl für Wanderer als auch für Spaziergänger gut machbar. Von Kufstein aus beträgt die Gehzeit etwa 45 Minuten. Alternativ kann man mit dem Auto bis zum Gasthof Neuhaus fahren, von wo aus der Turm in ca. 20 Minuten zu Fuß erreichbar ist. Der Weg ist gut ausgeschildert und führt durch eine idyllische Waldlandschaft.</p>
      <p class="my-3">Für Naturliebhaber, Geschichtsinteressierte und alle, die eine beeindruckende Aussicht genießen möchten, ist der Thierberg Turm ein lohnendes Ziel!</p>
      <Gallery items={images} class="gap-4 grid-cols-2 md:grid-cols-3" />
</div>
