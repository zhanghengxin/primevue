<template>
    <DocSectionText v-bind="$attrs">
        <p>Buttons can be placed at either side of an input element.</p>
    </DocSectionText>
    <div class="card flex flex-column md:flex-row gap-3">
        <InputGroup>
            <Button label="Search" />
            <InputText placeholder="Keyword" />
        </InputGroup>

        <InputGroup>
            <InputText placeholder="Keyword" />
            <Button icon="pi pi-search" severity="warning" />
        </InputGroup>

        <InputGroup>
            <Button icon="pi pi-check" severity="success" />
            <InputText placeholder="Vote" />
            <Button icon="pi pi-times" severity="danger" />
        </InputGroup>
    </div>
    <DocSectionCode :code="code" />
</template>

<script>
export default {
    data() {
        return {
            code: {
                basic: `
<InputGroup>
    <Button label="Search" />
    <InputText placeholder="Keyword" />
</InputGroup>

<InputGroup>
    <InputText placeholder="Keyword" />
    <Button icon="pi pi-search" severity="warning" />
</InputGroup>

<InputGroup>
    <Button icon="pi pi-check" severity="success" />
    <InputText placeholder="Vote" />
    <Button icon="pi pi-times" severity="danger" />
</InputGroup>
`,
                options: `
<template>
    <div class="card flex flex-column md:flex-row gap-3">
        <InputGroup>
            <Button label="Search" />
            <InputText placeholder="Keyword" />
        </InputGroup>

        <InputGroup>
            <InputText placeholder="Keyword" />
            <Button icon="pi pi-search" severity="warning" />
        </InputGroup>

        <InputGroup>
            <Button icon="pi pi-check" severity="success" />
            <InputText placeholder="Vote" />
            <Button icon="pi pi-times" severity="danger" />
        </InputGroup>
    </div>
</template>
`,
                composition: `
<template>
    <div class="card flex flex-column md:flex-row gap-3">
        <InputGroup>
            <Button label="Search" />
            <InputText placeholder="Keyword" />
        </div>

        <InputGroup>
            <InputText placeholder="Keyword" />
            <Button icon="pi pi-search" severity="warning" />
        </div>

        <InputGroup>
            <Button icon="pi pi-check" severity="success" />
            <InputText placeholder="Vote" />
            <Button icon="pi pi-times" severity="danger" />
        </div>
    </div>
</template>
`
            }
        };
    }
};
</script>
