<svelte:head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Informationen zum Thierberg Turm – Thierberger Schützen</title>
  <meta name="description" content="Erfahren Sie alles über den Thierberg Turm – Geschichte, Nutzung und Besichtigungsmöglichkeiten in Kufstein.">
  <meta name="keywords" content="Thierberger Schützen, Schützenturm, Informationen, Geschichte, Kufstein, Besichtigung, Tradition, Öffnungszeiten, Gehdauer, Startpunkt, Navigation">
  <meta name="author" content="Thierberger Schützen">
  <meta property="og:title" content="Informationen zum  Thierberg Turm – Thierberger Schützen">
  <meta property="og:description" content="Der  Thierberg Turm – ein historisches Wahrzeichen in Kufstein. Erfahren Sie mehr über seine Geschichte und Nutzung.">
  <meta property="og:url" content="https://www.thierberger-schuetzen.at/turm/informationen">
  <meta property="og:type" content="website">
  <meta property="og:image" content="/images/turm/turm3.jpg">
</svelte:head>

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
