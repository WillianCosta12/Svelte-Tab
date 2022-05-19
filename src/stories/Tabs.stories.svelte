<script>
    import { Meta, Template, Story } from "@storybook/addon-svelte-csf";
    import Tabs from "../components/Tabs.svelte";
</script>

<Meta 
    title="Tab/Tabs"
    component={Tabs}
/>

<Template let:args>
    <Tabs
    {...args}
    />
</Template>

<Story
  name="Tabs"
  args={{
    ids: [
          "Tab-01",
          "Tab-02",
          "Tab-03",
          "Tab-04"
        ],
    contents: [
        'Esse é o texto da Primeira Tab',
        'Esse é o texto da Segunda Tab',
        'Esse é o texto da Terceira Tab',
        'Esse é o texto da Quarta Tab'
    ]
  }}
/>

