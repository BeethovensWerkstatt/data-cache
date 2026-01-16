# data-cache

This repository contains files created by GitHub CI to avoid client-side processing.

## Workflow Description

A GitHub workflow in the [BeethovensWerkstatt/data](https://github.com/BeethovensWerkstatt/data) project automatically renders MEI files into SVG files using the [BeethovensWerkstatt/thulemeier](https://github.com/BeethovensWerkstatt/thulemeier) project. This happens server-side, so the rendering load doesn't need to be transferred to the client.

The workflow currently operates in the `dev` branch of the data repository and is triggered whenever changes are made:

### Processed File Types

- **Annotated Transcriptions**: Rendered into SVG
- **Diplomatic Transcriptions**: Rendered into SVG
- **Fluid Transcriptions**: Created using the [BeethovensWerkstatt/liquifier](https://github.com/BeethovensWerkstatt/liquifier) project, showing an animation between the two transcription types

The generated files are provided in this repository for direct use.

