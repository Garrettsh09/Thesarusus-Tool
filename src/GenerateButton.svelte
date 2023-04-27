<script lang="ts" context='module'>
    import { Form, FormGroup, FormText, Input, Label, Col, Row, Button, Fade, Card } from 'sveltestrap';
    import Sentence from './Sentence.svelte';

    export let word = 'Word';
</script>

<Form>
    <Row>
        <Col>
            <FormGroup>
                <Input type='text' name='text' placeholder="type here" bind:value={word}/>
                <h1> </h1>
                <Button color="primary" id="toggler" class="mb-3">Generate</Button>
                <Fade toggler="#toggler">
                    <Sentence sentence={word}/>
                </Fade>
            </FormGroup>
        </Col>
    </Row>
</Form>
