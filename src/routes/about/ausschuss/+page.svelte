<div class="bg-gray-100 px-8 py-2 rounded-xl">
    <h2 class="text-2xl md:text-3xlfont-extrabold dark:text-white my-3">Ausschuss</h2>
    
    <div class="card-container">
        <div class="myCard">
            <img class="placeholder" alt="Auschuss Mitglied" src="https://placehold.co/400x400"/>
            <h3 class="name">Ausschuss Mitglied 1</h3>
            <p class="function">Funktion</p>
        </div>
        
        <div class="myCard">
            <img class="placeholder" alt="Auschuss Mitglied" src="https://placehold.co/400x400"/>
            <h3 class="name">Ausschuss Mitglied 2</h3>
            <p class="function">Funktion</p>
        </div>
    
    </div>

</div>



<style>
    .placeholder{
        @apply rounded-lg
    }
    .myCard {
        @apply bg-gray-200 p-3 rounded-lg
    }

    .card-container{
        @apply grid grid-cols-4 gap-3
    }

    .name{
        @apply text-xl font-semibold my-2
    }

    .function{

    }
</style>