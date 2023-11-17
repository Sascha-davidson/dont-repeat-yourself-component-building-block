<form action="">
  <div class="input-container">
    <label for="PlayerName">Player Name ... </label>
    <input type="text" id="PlayerName" placeholder="Place your name" />
  </div>
  <section>
    <div class="input-container">
      <label for="BirthDate">Date of birth ...</label>
      <input type="date" id="BirthDate" />
    </div>
    <div class="input-container">
      <label for="JerseyNumber">Jersey number ...</label>
      <input type="text" id="JerseyNumber" />
    </div>
  </section>
  <div class="input-container">
    <label for="BirthCountry">Country of birth ...</label>
    <input type="text" id="BirthCountry" />
  </div>
  <div class="input-container">
    <label for="ResidencePlace">Place of residence ...</label>
    <input type="text" id="ResidencePlace" />
  </div>
  <div class="input-container">
    <label for="Bio">Bio ...</label>
    <input type="text" id="Bio" />
  </div>
</form>

<style>
  form {
    display: flex;
    flex-direction: column;
    gap: 2rem;
  }

  section {
    display: flex;
    gap: 2rem;
  }

  div{
    position: relative;
  }

  label {
    position: absolute;
    top: 50%;
    left: 2rem;
    right: 2rem;
    transform: translateY(-50%);
    transition: 0.3s ease-in-out;
  }

  input {
    padding: 1rem 2rem;
    border-radius: 0.9rem;
    /* border: 3px solid white; */
    border: none;
    outline: 3px solid white;
    outline-offset: -3px;
    box-shadow: var(--box-shadow);
    font-size: 1rem;
    width: 100%;
    color: var(--text-color);
  }

div input + label{

}
</style>
