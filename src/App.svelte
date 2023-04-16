<script lang="ts">
	import { Col, Container, Row } from 'sveltestrap';
    import Generate from './GenerateButton.svelte';
	import Sentence from './Sentence.svelte';
	import NextPreviousButton from './NextPreviousButton.svelte';
</script>

<style>
	:global(main){
	  font-family: monospace;
	  text-align: center;
	  color: rgb(69, 191, 69);
	  background-color: rgb(194, 184, 173);
	  font-size: 1em;
	}

	@media(max-width: 700px){
		:global(.search){
			margin-top: 0;
			
		}
	}
</style>

<main>
	<Container>
		<Row>
			<Col>
				<h1>Thesaurus Tool</h1>
			</Col>
		</Row>
		<Generate/>
		<Row>
			<Col>
				<Sentence sentence='Select the word you want to choose' />
				<h1> </h1>
			</Col>
		</Row>
		<NextPreviousButton/>
	</Container>
</main>

