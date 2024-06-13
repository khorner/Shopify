# Introduction to Shopify CLI Hands-On Lab

## Overview

Welcome to the **Introduction to Shopify CLI** hands-on lab! In this lab, you will learn how to use the Shopify CLI (Command Line Interface) to interact with your Shopify store. By the end of this lab, you will be able to add products to an existing store using the Shopify CLI.

## Objectives

- Understand the basics of Shopify CLI
- Set up the Shopify CLI on your local machine
- Authenticate and connect to your Shopify store
- Add products to your Shopify store using the CLI

## Prerequisites

Before you begin, ensure you have the following:

- A Shopify store
- Node.js installed on your machine
- npm (Node Package Manager) installed
- Basic knowledge of command-line operations

## Contents

This lab is divided into the following sections:

1. [Setting Up Shopify CLI](#setting-up-shopify-cli)
2. [Authenticating and Connecting to Your Store](#authenticating-and-connecting-to-your-store)
3. [Adding Products Using Shopify CLI](#adding-products-using-shopify-cli)
4. [Troubleshooting and Tips](#troubleshooting-and-tips)

## Setting Up Shopify CLI

1. **Install Shopify CLI**:
    ```sh
    npm install -g @shopify/cli @shopify/theme
    ```

2. **Verify Installation**:
    ```sh
    shopify version
    ```

    You should see the version number of Shopify CLI printed in your terminal.

## Authenticating and Connecting to Your Store

1. **Login to Shopify**:
    ```sh
    shopify login
    ```

    Follow the instructions to log in to your Shopify account.

2. **Connect to Your Store**:
    ```sh
    shopify store connect
    ```

    Enter your store domain when prompted.

## Adding Products Using Shopify CLI

1. **Create a Product**:
    ```sh
    shopify product create --title "New Product" --price 19.99
    ```

    Replace `"New Product"` with the name of your product and `19.99` with the price of your product.

2. **List Products**:
    ```sh
    shopify product list
    ```

    This command lists all products in your store, confirming that your new product has been added successfully.

## Troubleshooting and Tips

- **Command Not Found**: If you encounter a `command not found` error, ensure that the Shopify CLI is installed correctly and that your PATH environment variable includes npm global packages.
- **Authentication Issues**: Ensure that you are using the correct credentials and that you have the necessary permissions to access the store.
- **More Help**: For more detailed information and advanced usage, refer to the [Shopify CLI Documentation](https://shopify.dev/docs/api/shopify-cli).

## Conclusion

Congratulations! You have successfully completed the Introduction to Shopify CLI lab. You have learned how to set up Shopify CLI, authenticate and connect to your store, and add products using the CLI. Keep exploring the Shopify CLI to further enhance your store management capabilities.

## Resources

- [Shopify CLI Documentation](https://shopify.dev/docs/api/shopify-cli)
- [Shopify Dev Documentation](https://shopify.dev/docs)

---

**Maintained by [Your Organization]**
