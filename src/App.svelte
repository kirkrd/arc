<script lang="ts">
    import AppContainer from "./lib/AppContainer.svelte";
    import CarApp from "./lib/CarApp.svelte";
    import CarSide from "./assets/carside.png"
</script>

<main>
    <div>
    <img class="car-image" src={CarSide} alt="sport car from the side" />
    </div>
   <AppContainer>
        <CarApp />
    </AppContainer>
</main>

<style>
    main {
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .car-image {
        max-width: 400px;
    }
</style>
