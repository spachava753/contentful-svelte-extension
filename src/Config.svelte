<script>
    export let sdk;
    let name = "world";
    const app = sdk.app;
    app.setReady();
</script>

<h1>
    This is the config screen
</h1>

<p>Hello {name}</p>

<input type="text" bind:value={name}>