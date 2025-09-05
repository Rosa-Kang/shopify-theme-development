# Shopify Theme Project

This repository contains the source code for a custom Shopify theme. It includes all the necessary assets, templates, and configuration files to create a unique storefront experience. This project is set up to be developed and deployed using the Shopify CLI.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Local Development](#local-development)
- [Shopify CLI Commands](#shopify-cli-commands)
- [Directory Structure](#directory-structure)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

Before you begin, ensure you have the following installed:

- [Shopify CLI](https://shopify.dev/docs/cli)
- [Node.js and npm](https://nodejs.org/)
- A Shopify partner account and a development store.

## Local Development

To set up and run this theme on your local machine, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone <your-repository-url>
    cd shopify-theme
    ```

2.  **Connect to your Shopify store:**
    Log in to your Shopify account and connect to your desired store. You will be prompted to authenticate in your web browser.
    ```bash
    shopify login --store YOUR_STORE_NAME.myshopify.com
    ```

3.  **Start the local development server:**
    This command starts a local server that mimics the Shopify theme environment. It automatically watches for changes to your files and enables hot-reloading.
    ```bash
    shopify theme dev
    ```
    Once running, the CLI will output a URL to preview your local theme on the development store.

## Shopify CLI Commands

This theme is managed using the Shopify CLI. Here are some of the most common commands:

- `shopify theme dev`: Starts the local development server with hot-reloading.
- `shopify theme check`: Checks the theme for errors, performance issues, and best practice violations.
- `shopify theme push`: Pushes your local changes to a specific theme on your Shopify store.
- `shopify theme pull`: Pulls the latest version of a theme from your Shopify store to your local environment.

## Directory Structure

The project follows the standard Shopify theme directory structure:

-   `assets/`: Contains all theme assets such as CSS, JavaScript, images, and icons.
-   `config/`: Holds the theme's configuration files, including `settings_schema.json` (defines the Theme Editor settings) and `settings_data.json` (stores the saved settings).
-   `layout/`: Contains the main layout file, `theme.liquid`, which acts as the global template for the store.
-   `locales/`: Stores translation files (in JSON format) for internationalizing the theme.
-   `sections/`: Contains Liquid files that represent reusable modules of content for a page (e.g., header, footer, featured product).
-   `snippets/`: Holds smaller, reusable pieces of Liquid code that can be included in other files.
-   `templates/`: Contains the main Liquid templates for different page types, such as products, collections, and customer accounts.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the [MIT License](LICENSE).
