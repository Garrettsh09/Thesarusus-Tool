<script lang="ts">
	import { Col, Container, Row } from 'sveltestrap';
    import Generate from './GenerateButton.svelte';
</script>

<style>
	:global(main){
	  font-family: monospace;
	  text-align: center;
	  color: green;
	  background-color: rgb(194, 184, 173);
	  font-size: 1em;
	}
</style>

<main>
	<Container>
		<Row>
			<Col>
				<h1>Thesarusus Tool</h1>
			</Col>
		</Row>
		<Generate/>
	</Container>
</main>

