<script lang="ts" context='module'>
    import { Form, FormGroup, FormText, Input, Label, Col, Row, Button } from 'sveltestrap';
    let word;
    export let disp;
    disp = 'a'

    function hasSent(){
        const disp = word;   
    };

</script>

<Form>
    <Row>
        <Col>
            <FormGroup>
                <h1> </h1>
                <Input type="text"  bind:value={word} placeholder='Placeholder'/>
                <h1> </h1>
                <Button color="primary" class="Generate" on:click={hasSent}>Generate </Button>
            </FormGroup>
        </Col>
    </Row>
</Form>
