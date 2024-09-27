<script>
	import { useForm, validators, HintGroup, Hint, email, required } from "svelte-use-form";

	const form = useForm();


	let data = undefined
</script>

<main>


	<form use:form method="POST" action="/login">
		<h1>Login</h1>

		<input type="email" name="email" use:validators={[required, email]} />
		<HintGroup for="email">
			<Hint on="required">This is a mandatory field</Hint>
			<Hint on="email" hideWhenRequired>Email is not valid</Hint>
		</HintGroup>

		<input type="password" name="password" use:validators={[required]} />
		<Hint for="password" on="required">This is a mandatory field</Hint>

		<button disabled={!$form.valid} formaction="/login">Login</button>
		<button formaction="?/register">Register</button>
	</form>

	<a href="/register">You don't have an account? Sign up</a>

</main>

<style>
main {
	display: block;
	margin-top: 15em;
	justify-content: center;
}
:global(.touched:invalid) {
		border-color: red;
		outline-color: red;
	}
</style>
