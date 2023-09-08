<script>
  import Alert from "./components/alert.svelte";
import Button from "./components/button.svelte";
    import ButtonGroup from "./components/buttonGroup.svelte";
    import Input from "./components/input.svelte";
    import Widget from "./components/widget.svelte";
</script>

<main>
  <Button  color="primary" disabled>click me!</Button>
  <ButtonGroup space="200px" direction="row">
    <Button on:click={() => console.log("hello world")} color="warning">click me!</Button>
    <Button type="outline" color="success">click me!</Button>
    <Button type="outline" color="alert">click me!</Button>
  </ButtonGroup>
  <Widget>
    <Button>hii</Button>
    <Alert color="alert">
      yo 
    </Alert>
  </Widget>
  <Alert color="success">
    hello world !
  </Alert>
  <Input placeholder="yo"/>
</main>
