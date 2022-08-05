<script>
import Confirm from '$lib/Confirm.svelte';

function deleteItem() {
    alert('Deleted')
}
</script>

<h1>Welcome to SvelteKit</h1>

<Confirm confirmTitle="Delete" cancelTitle="Cancel" let:confirm="{confirmThis}">
    <button on:click={() => confirmThis(deleteItem)}>Delete</button>
</Confirm>
