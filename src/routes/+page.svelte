<script>
  import Nav from "$lib/nav/Nav.svelte";
  import SaveNext from "$lib/buttons/save-next.svelte";
  import Form from "$lib/form/form.svelte";
</script>

<div>
  <main>
    <h2 id="title">Create Player</h2>
    <p class="CreatePlayer">Create a player</p>
    <p class="AddPlayer">Add player to team</p>
    <Form />

    <p class="other">other data</p>
    <SaveNext />
  </main>

  <Nav />
</div>

<style>
  div {
    display: flex;
    height: 100%;
  }

  main {
    height: 100%;
    width: 100%;
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: auto auto 1fr auto;
    column-gap: 2rem;
    row-gap: 0;
    padding: 4rem 7%;
    grid-template-areas:
      "Title Title"
      "CreatePlayer AddPlayer"
      "form other"
      "button button";
  }

  h2 {
    grid-area: Title;
    padding: 1rem;
  }

  p{
    padding: 1rem;
  }

  .CreatePlayer {
    grid-area: CreatePlayer;
  }

  .AddPlayer {
    grid-area: AddPlayer;
  }

  .form {
    grid-area: form;
  }

  .other {
    grid-area: other;
  }

  button{
    grid-area: button;
  }
</style>
