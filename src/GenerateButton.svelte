<script lang="ts">
    import { Form, FormGroup, FormText, Input, Label, Col, Row, Button } from 'sveltestrap';
</script>

<Form>
    <Row>
        <Col>
            <FormGroup>
                <Input type="text" id="Generate" placeholder="Put your sentence here"/>
                <h1> </h1>
                <Button color="primary" class="Generate">Generate</Button>
            </FormGroup>
        </Col>
    </Row>
</Form>
