<script>
  import Nav from "$lib/nav/Nav.svelte";
</script>

<div>
  <main>
    <h2 id="title">Create Player</h2>
    <p class="CreatePlayer">Create a player</p>
    <p class="AddPlayer">Add player to team</p>
    <form action="" />
    <p class="other">other</p>
    <button>save</button>
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
    gap: 2rem;
    padding: 8rem 10%;
    grid-template-areas:
      "Title Title"
      "CreatePlayer AddPlayer"
      "form other"
      "button button";
  }

  h2 {
    grid-area: Title;
  }

  .CreatePlayer {
    grid-area: CreatePlayer;
  }

  .AddPlayer {
    grid-area: AddPlayer;
  }

  form {
    grid-area: form;
    border-radius: 1.5rem;
  }

  .other {
    grid-area: other;
  }

  button{
    grid-area: button;
    height: fit-content;
    width: fit-content;
    padding: 1rem 2rem;
    border-radius: 50rem;
    background-color: #63C6A7;
    color: white;
    border: none;
  }
</style>
