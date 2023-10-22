# Typescript Types for Dialogflow CX Messenger Integration

Typescript classes and types to use Dialogflow Messenger Types in Typescript.

## Installation

To install:
```bash
npm install dialogflow-cx-messenger-ts
```
or
```bash
yarn add dialogflow-cx-messenger-ts
```

## Usage
Once installed, you can import the types and use them in your code:
```typescript
import * as dfcxmessenger from 'dialogflow-cx-messenger-ts';
```

Then you can use it to create a response:
```typescript

  const response = {};

  const content = new dfcxmessenger.RichContent();
  const richContentElement = new dfcxmessenger.RichContentElement();
  richContentElement.type = "image";
  richContentElement.rawUrl = sprite;
  richContentElement.accessibilityText = "Example logo";
  content.richContent = [[richContentElement]];

  response.fulfillmentResponse = {
    messages: [{
      text: {
        text: [
          information,
        ],
      },
    },
    {
      payload: content,
    }],
  };
```

## Documentation
You can find the documentation [here](https://xavidop.github.io/dialogflow-cx-messenger-ts/).

## Example
You can find an example [here](https://github.com/xavidop/dialogflow-cx-webhook-pokedex)

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please make sure that read the [Contributing](CONTRIBUTING.md) file.

## Sponsors

Does your company use this package? Help keep the project bug-free and feature rich by [sponsoring the project](https://github.com/sponsors/xavidop).

<a href="https://github.com/sponsors/xavidop" target="_blank"><img src="https://opencollective.com/cxcli/sponsors/0/avatar"></a>

## Contributors

This project exists thanks to all the people who contribute. Check our [contributing guidelines](CONTRIBUTING.md).
Check all contributors [here](https://github.com/xavidop/dialogflow-cx-messenger-ts/graphs/contributors).

## Stargazers over time

[![Stargazers over time](https://starchart.cc/xavidop/dialogflow-cx-messenger-ts.svg)](https://starchart.cc/xavidop/dialogflow-cx-messenger-ts)


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fxavidop%2Fdialogflow-cx-messenger-ts.svg?type=large&issueType=license)](https://app.fossa.com/projects/git%2Bgithub.com%2Fxavidop%2Fdialogflow-cx-messenger-ts?ref=badge_large&issueType=license)