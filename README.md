# @postiva/client

[![npm version](https://badge.fury.io/js/%40postiva%2Fclient.svg)](https://badge.fury.io/js/%40postiva%2Fclient)
[![GitHub license](https://img.shields.io/github/license/postiva/client)](https://github.com/postiva/postiva-js/blob/main/LICENSE)

## Introduction

Welcome to `@postiva/client` – a powerful library crafted to empower developers in effortlessly managing and retrieving content within their applications. With a simple yet robust API, it seamlessly interacts with the Postiva platform, ensuring your content remains consistently accessible and updated.

## Features

- **Effortless Content Management**: Seamlessly fetch and manage content within your application.
- **Pagination Support**: Handle large datasets effectively with built-in pagination support.
- **Secure Authentication**: Utilize secure API keys for authentication to ensure data integrity.
- **Custom Queries**: Fetch content based on specific criteria using custom queries.
- **REST API Support**: Integrate your blog seamlessly into any tech stack with REST API support.

## Installation

You can install `@postiva/client` via npm, yarn, or pnpm:

```bash
npm install @postiva/client
```

## Usage

To start using `@postiva/client` in your project, initialize the client by providing your workspace ID and API key:

```js
import { createClient } = from "@postiva/client"

// Initialize Postiva Client
const client = createClient('yourWorkspaceId', 'yourApiKey');
```

### Rest API Documentation

The REST API documentation for `@postiva/client` has been automatically generated by Bruno. Please refer to **REST API Documentation** for details.

### Official Documentation

For more comprehensive usage examples and detailed API documentation, please visit the [official documentation](https://docs.postiva.app/).

## Contributing

Contributions to `@postiva/client` are welcome! If you have ideas for improvements, found a bug, or want to contribute new features, please check out our contribution guidelines and code of conduct before opening an issue or submitting a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Support
For support or inquiries, please contact us at help@postiva.app.