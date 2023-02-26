<script lang="ts">
    import ProductCard from "$lib/productCard.svelte";

    const products : Product[] = [
        {
            id: "1",
            name: "Donut",
            price: 5.4
        },
        {
            id: "2",
            name: "Other Donut",
            price: 5.9
        },
    ]
</script>

<div class="container h-full mx-auto flex justify-center items-center">
    <div class="grid grid-cols-3 gap-4">
        <div class="col-span-3">
            <h1>DDDDonuts!</h1>
        </div>
        {#each products as product}
            <ProductCard product = {product}/>
        {/each}
    </div>
</div>
