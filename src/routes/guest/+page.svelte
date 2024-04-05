<script>
	import { goto } from "$app/navigation";

	const toggleSignIn = () => goto("/");
	const toggleSignUp = () => goto("/sign-up");
</script>

<div class="sign-in-up-container">
	<button class="sign-in-btn" on:click={toggleSignIn}>Sign-in</button>
	<button class="sign-up-btn" on:click={toggleSignUp}>Sign-up</button>
</div>
<div class="app-header">Wongnok Recipes</div>
