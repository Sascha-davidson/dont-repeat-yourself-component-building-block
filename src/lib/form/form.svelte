<form id="style-2" action="">
  <div class="input-container">
    <input type="text" id="PlayerName" placeholder="" required />
    <label for="PlayerName">Player Name ... </label>
  </div>
  <section>
    <div class="input-container active">
      <input type="date" id="BirthDate" placeholder="" />
      <label for="BirthDate">Date of birth ...</label>
    </div>
    <div class="input-container">
      <input type="text" id="JerseyNumber" placeholder="" required />
      <label for="JerseyNumber">Jersey number ...</label>
    </div>
  </section>
  <div class="input-container">
    <input type="text" id="BirthCountry" placeholder="" />
    <label for="BirthCountry">Country of birth ...</label>
  </div>
  <div class="input-container">
    <input type="text" id="ResidencePlace" placeholder="" />
    <label for="ResidencePlace">Place of residence ...</label>
  </div>
  <div class="input-container">
    <textarea id="Bio" placeholder="" />
    <label for="Bio">Bio ...</label>
  </div>
</form>

<style>
  form {
    display: flex;
    flex-direction: column;
    gap: 2.5rem;
    padding: .5rem 1rem;
    overflow: auto;
    padding-top: 1.5rem;
  }

  #style-2::-webkit-scrollbar-track
{
	border-radius: 10px;
}

#style-2::-webkit-scrollbar
{
	width: 12px;
}

#style-2::-webkit-scrollbar-thumb
{
	border-radius: 10px;
	/* -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,.3); */
	background-color: #a7a7a7;
}

  section {
    display: flex;
    gap: 2rem;
  }

  div {
    position: relative;
    width: 100%;
  }

  label {
    position: absolute;
    top: 1rem;
    left: 1.5rem;
    transition: 0.3s ease-in-out;
    cursor: text;
  }

  input {
    padding: 1rem 1.5rem;
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

  div input:focus ~ label,
  div input:not(:placeholder-shown) ~ label {
    top: -1.3rem;
    font-size: 12px;
  }

  .active label {
    top: -1.3rem;
    font-size: 12px;
  }

  div textarea{
    height: 6rem;
    width: 100%;
    padding: 1rem 1.5rem;
    font-size: 1rem;
    font-family: Arial, Helvetica, sans-serif;
    color: var(--text-color);

    border: none;
    outline: 3px solid white;
    outline-offset: -3px;
    box-shadow: var(--box-shadow);
    border-radius: 0.9rem;
  }

  div textarea:focus ~ label,
  div textarea:not(:placeholder-shown) ~ label {
    top: -1.3rem;
    font-size: 12px;
  }
</style>
