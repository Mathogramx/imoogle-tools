<div align="center">
        <img src="src/assets/logo.png" width="220" />
        <br /><br />
        <h1>imoogletools</h1>
        <p><em>by imoogle technology</em></p>
        <br />
</div>

Welcome to imoogletools, a self-hosted web app offering a variety of online tools to simplify everyday tasks.
Whether you are coding, manipulating images/videos, PDFs or crunching numbers, imoogletools has you covered.
Developed by imoogle technology to provide powerful tools for everyone.

All files are processed entirely on the client side: nothing ever leaves your device.
Plus, the Docker image is super lightweight at just 28MB, making it fast to deploy and easy to self-host.

![img.png](docs-images/img.png)

## Table of Contents

- [Features](#features)
- [Self-host](#self-hostrun)
- [Contribute](#contribute)
- [Contact](#contact)
- [License](#license)

## Features

We strive to offer a variety of tools, including:

### **Image/Video/Audio Tools**

- Image Resizer
- Image Converter
- Image Editor
- Video Trimmer
- Video Reverser
- And more...

### **PDF Tools**

- PDF Splitter
- PDF Merger
- PDF Editor
- And more...

### **Text/List Tools**

- Case Converters
- List Shuffler
- Text Formatters
- And more...

### **Date and Time Tools**

- Date Calculators
- Time Zone Converters
- And more...

### **Math Tools**

- Generate Prime Numbers
- Calculate voltage, current, or resistance
- And more...

### **Data Tools**

- JSON Tools
- CSV Tools
- XML Tools
- And more...

Stay tuned as we continue to expand and improve our collection!

## Self-host/Run

### Docker

```bash
docker run -d --name imoogletools --restart unless-stopped -p 8080:80 imoogletools:latest
```

### Docker Compose

```yaml
services:
  imoogletools:
    image: imoogletools:latest
    container_name: imoogletools
    restart: unless-stopped
    ports:
      - "8080:80"

```

## Development

This is a React Project with Typescript Material UI. We use icons from [Iconify](https://icon-sets.iconify.design)

### Project setup

```bash
git clone <repository-url>
cd imoogletools
npm i
npm run dev
```

### Create a new tool

```bash
npm run script:create:tool my-tool-name folder1 # npm run script:create:tool split pdf
```

For tools located under multiple nested directories, use:

```bash
npm run script:create:tool my-tool-name folder1/folder2 # npm run script:create:tool compress image/png
```

Use `folder1\folder2` on Windows.

### Run tests

```bash
npm run test
```

- For e2e tests

```bash
npm run test:e2e
```

### i18n (Translations)
The translation files are [here](public/locales).

## Contact

For any questions or suggestions, feel free to contact imoogle technology at:
[contact@imoogle.tech](mailto:contact@imoogle.tech)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
