# ComfyUI Documentation

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify) to preview the documentation changes locally. To install, use the following command

```
npm i mintlify
```

Run the following command at the root of your documentation (where mint.json is)

```
npx mintlify dev
```

### Create a PR

Create a PR. Once it is accepted Vercel will deploy the change to https://docs.comfy.org/

### Generating API Reference Docs

Can either use an OpenAPI file or URL containing the file:

```bash
cd registry/api-reference # Keep API files separated by products.
npx @mintlify/scraping@latest openapi-file <path-to-openapi-file>
```

This will only generate the MDX files for each endpoint. You need to add a link to these files in `mint.json`, and the up-to-date API spec will be shown on that doc page.

## Contributing

Please just create a PR and we will review it within a few days.

Or talk to us on our [discord](https://discord.com/invite/comfyorg) :)

## Custom Nodes Documentation

The following files provide detailed documentation for custom nodes:

- [Code Interface](essentials/custom_node_interface.mdx)
- [Lifecycle](essentials/custom_node_lifecycle.mdx)
- [Hidden and Flexible Inputs](essentials/custom_node_more_on_inputs.mdx)
- [Overview](essentials/custom_node_overview.mdx)
- [Server Overview](essentials/custom_node_server_overview.mdx)
- [Annotated Examples](essentials/custom_node_snippets.mdx)
- [Working with torch.Tensor](essentials/custom_node_tensors.mdx)
- [Step-by-Step Walkthrough](essentials/custom_node_walkthrough.mdx)
