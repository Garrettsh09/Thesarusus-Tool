<script>
    import { onMount } from 'svelte';
    import { Form, FormGroup, FormText, Input, Label, Col, Row, Button } from 'sveltestrap';
    let word;

    onMount (async() =>{
        const response = await fetch('https://wordprobe-wordprobe-v1.p.rapidapi.com/synonyms/bright', {
	        method: 'GET',
	        headers: {
		    'X-RapidAPI-Key': '28f74b09f9msh061e54d6ddd1897p15bd7cjsn2e2f3d415bac',
		    'X-RapidAPI-Host': 'wordprobe-wordprobe-v1.p.rapidapi.com',
	        },
	    }
        
        );
        const data = await response.json();
        word = data.WordProbe;
    });

</script>

<Form>
    <Row>   
        <h1>{word}</h1>
    </Row>
</Form>
