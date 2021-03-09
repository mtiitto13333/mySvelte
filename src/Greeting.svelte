<script>
    export let firstName;
    export let lastName;
</script>

<label for="firstName">First Name</label><input name="firstName"
bind:value={firstName}>
<label for="lastName">Last Name</label><input name="lastName"
bind:value={lastName}>

<p>My name is <span>{firstName} {lastName}</span></p>
<style>
    h2 {
        color: blueviolet;
    }
    span {
        border-bottom: 1px solid;
        min-width: 10em;
        display: inline-block;
    }
</style>