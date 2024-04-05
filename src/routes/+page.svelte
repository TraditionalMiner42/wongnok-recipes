<script>
	import { goto } from "$app/navigation";

	const directToMemberPage = () => goto("/member");
	const directToGuestPage = () => goto("/guest");
</script>

<div class="app-header px-4 py-2 m-4">Wongnok Recipes</div>
<div class="form-container">
	<form class="sign-in-container" method="post">
		<input class="email-input" placeholder="Enter your email" />
		<input class="pw-input" placeholder="Enter your password" />
		<button
			class="sign-in-btn mx-[25em]"
			on:click|preventDefault={directToMemberPage}>Sign In</button
		>
		<button
			class="sign-in-btn mx-[25em]"
			on:click|preventDefault={directToGuestPage}>View as Guest</button
		>
	</form>
</div>
