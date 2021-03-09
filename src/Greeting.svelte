<script>
    export let firstName;
    export let lastName;
</script>

<label for="firstName">First Name</label><input name="firstName"
bind:value={firstName}>
<label for="lastName">Last Name</label><input name="lastName"
bind:value={lastName}>

<p>My name is {firstName} {lastName}</p>
<style>
    h2 {
        color: blueviolet;
    }
</style>