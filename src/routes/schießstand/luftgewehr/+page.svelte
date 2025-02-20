<svelte:head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Luftgewehr Schießstand – Thierberger Schützen</title>
  <meta name="description" content="Der Luftgewehr-Schießstand der Thierberger Schützen bietet optimale Trainingsbedingungen für Anfänger und erfahrene Schützen in Kufstein.">
  <meta name="keywords" content="Thierberger Schützen, Luftgewehr, Schießstand, Schießsport, Training, Kufstein, Schützenverein">
  <meta name="author" content="Thierberger Schützen">
  <meta property="og:title" content="Luftgewehr Schießstand – Thierberger Schützen">
  <meta property="og:description" content="Entdecken Sie den modernen Luftgewehr-Schießstand der Thierberger Schützen – ideale Trainingsmöglichkeiten für alle Leistungsstufen.">
  <meta property="og:url" content="https://www.thierberger-schuetzen.at/schießstand/luftgewehr">
  <meta property="og:type" content="website">
  <meta property="og:image" content="/images/other/ferien.jpeg">
</svelte:head>

<script>
    import { Gallery } from 'flowbite-svelte';
    const images = [
      { alt: 'Jasmin', src: '/images/other/jasmin.jpg' },
      { alt: 'Clown-Scheibe', src: '/images/other/clown.jpg' },
      { alt: 'Kinder in Faschingskostümen', src: '/images/other/krapfenschiessen.jpeg' },
      { alt: 'Unsre Schützen-Jugend', src: '/images/other/auswertung.jpeg' },
      { alt: 'Ferienexpress Kinder', src: '/images/other/ferien.jpeg' },
      { alt: 'Ferienexpress Kinder Gruppenfoto mit OSM', src: '/images/other/ferien2.jpeg' },

    ];
  </script>
  
  
  <div class="bg-gray-100 px-8 py-2 rounded-xl">
      <h2 class="text-2xl md:text-3xl font-extrabold dark:text-white my-3">Unser Luftgewehr Schießstand</h2>
      <p class="my-3">Unser Luftgewehrschießstand in Morsbach 71, Kufstein verfügt über acht moderne elektronische Stände mit DISAG-Anlagen, die ein präzises und zeitgemäßes Training ermöglichen. Hier treffen sich sowohl erfahrene Schützen als auch der Nachwuchs, um ihre Treffsicherheit zu verbessern und sich in einem geselligen Umfeld sportlich zu messen.</p>
      <p class="my-3">Besonderes Augenmerk legen wir auf die Jugendförderung: Jeden Freitag um 18:30 Uhr findet das Jugendtraining statt, bei dem junge Schützen den sicheren Umgang mit dem Luftgewehr erlernen und ihre Fertigkeiten unter Anleitung erfahrener Trainer verbessern können. Direkt im Anschluss beginnt um 19:30 Uhr das Saisonschießen, das in der Wintersaison zahlreiche Mitglieder und Gäste anlockt. Dabei sind nicht nur Schützen willkommen – auch wer selbst nicht schießen möchte, kann in geselliger Runde vorbeikommen. Oft findet sich eine nette Kartenrunde, die den Abend in gemütlicher Atmosphäre abrundet.</p>
      <p class="my-3">Neben dem sportlichen Wettkampf stehen auch gesellige Veranstaltungen im Mittelpunkt. Unser traditionelles Krapfenschießen, bei dem es leckere Faschingskrapfen zu gewinnen gibt, erfreut sich großer Beliebtheit. Ebenso zieht das Klotzenbrotschießen viele Teilnehmer an, die sich nicht nur am Schießen, sondern auch an dieser regionalen Spezialität erfreuen.</p>
      <Gallery items={images} class="gap-4 grid-cols-2 md:grid-cols-3" />
    </div>
