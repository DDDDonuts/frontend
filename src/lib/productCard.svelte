<script lang="ts">
    export let product : Product = {id: "", name: "", price: 0}
</script>

<div class="card">
    <header class="card-header">
        <h2>{product.name}</h2>
    </header>
    <div class="card-body px-4">
        Price: {product.price}$
    </div>
    <footer class="card-footer">
        <button class="p-2 rounded variant-glass-primary">Buy</button>
        <button class="p-2 rounded variant-glass-secondary">List</button>
    </footer>
</div>
