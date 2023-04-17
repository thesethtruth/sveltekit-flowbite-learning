<script>
    export let options = [];
    export let title = "Dropdown";

    import { Button, Chevron, Dropdown, DropdownItem } from "flowbite-svelte";
</script>

<Button><Chevron>{title}</Chevron></Button>
<Dropdown>
    {#each options as option}
        <DropdownItem>{option}</DropdownItem>
    {/each}
</Dropdown>
