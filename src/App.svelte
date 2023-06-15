<script>
  import { onMount } from 'svelte';

  import LandingPage from './LandingPage.svelte';
  import SelectedOption from './SelectedOption.svelte';
  import Navbar from './Navbar.svelte';

  let selectedOption = null;

  function selectOption(option) {
    selectedOption = option;
    currentPage = SelectedOption;
  }

  let currentPage;
  onMount(() => {
    currentPage = selectedOption ? SelectedOption : LandingPage;
  });
</script>

<main>
	<Navbar />
  <svelte:component this={currentPage} {selectedOption} {selectOption} />
</main>
