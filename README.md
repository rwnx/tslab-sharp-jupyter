# Quick Start

Set up Python environment and install dependencies:

```sh
pipenv install

# Add local node_modules to PATH to avoid global TSLab installation
echo 'export PATH="$PATH:$PWD/node_modules/.bin"' >> $(pipenv --venv)/bin/activate
pipenv shell
```

Install and configure TSLab:

```sh
npm i
npx tslab install
```

Start Jupyter:

```sh
jupyter lab
```

## Usage

Display images in notebooks:

```typescript
import * as tslab from "tslab";
tslab.display.html(
  `<img src="data:image/jpeg;base64,${result.toString("base64")}" />`
);
```

see also https://github.com/yunabe/tslab/blob/main/docs/advanced.md
