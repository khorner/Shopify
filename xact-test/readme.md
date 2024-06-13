# Creating Test Transactions with Shopify CLI Hands-On Lab

## Overview

Welcome to the **Creating Test Transactions with Shopify CLI** hands-on lab! In this lab, you will learn how to use the Shopify CLI to create and manage test orders in your Shopify store. By the end of this lab, you will be able to create an order in an existing store using the CLI.

## Objectives

- Understand the basics of creating test orders using Shopify CLI
- Set up the Shopify CLI on your local machine
- Authenticate and connect to your Shopify store
- Create and manage test orders using the CLI

## Prerequisites

Before you begin, ensure you have the following:

- A Shopify store (preferably a development store)
- Node.js installed on your machine
- npm (Node Package Manager) installed
- Basic knowledge of command-line operations

## Contents

This lab is divided into the following sections:

1. [Setting Up Shopify CLI](#setting-up-shopify-cli)
2. [Authenticating and Connecting to Your Store](#authenticating-and-connecting-to-your-store)
3. [Creating Test Orders Using Shopify CLI](#creating-test-orders-using-shopify-cli)
4. [Managing Test Orders](#managing-test-orders)
5. [Troubleshooting and Tips](#troubleshooting-and-tips)

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

## Creating Test Orders Using Shopify CLI

1. **Create a Test Order**:
    ```sh
    shopify order create --product "Product Name" --quantity 1 --customer-email "customer@example.com"
    ```

    Replace `"Product Name"` with the name of an existing product in your store and `"customer@example.com"` with a test customer email.

2. **View the Test Order**:
    ```sh
    shopify order list
    ```

    This command lists all orders in your store, including the newly created test order.

## Managing Test Orders

1. **Mark Order as Fulfilled**:
    ```sh
    shopify order fulfill --order-id <order-id>
    ```

    Replace `<order-id>` with the ID of the test order you created.

2. **Cancel a Test Order**:
    ```sh
    shopify order cancel --order-id <order-id>
    ```

    Replace `<order-id>` with the ID of the test order you want to cancel.

3. **Delete a Test Order**:
    ```sh
    shopify order delete --order-id <order-id>
    ```

    Replace `<order-id>` with the ID of the test order you want to delete.

## Troubleshooting and Tips

- **Command Not Found**: If you encounter a `command not found` error, ensure that the Shopify CLI is installed correctly and that your PATH environment variable includes npm global packages.
- **Authentication Issues**: Ensure that you are using the correct credentials and that you have the necessary permissions to access the store.
- **More Help**: For more detailed information and advanced usage, refer to the [Shopify CLI Documentation](https://shopify.dev/docs/apps/build/orders-fulfillment/order-management-apps/manage-test-orders) and [Shopify Test Orders Documentation](https://help.shopify.com/en/partners/dashboard/managing-stores/test-orders-in-dev-stores).

## Conclusion

Congratulations! You have successfully completed the Creating Test Transactions with Shopify CLI lab. You have learned how to set up Shopify CLI, authenticate and connect to your store, create test orders, and manage those orders using the CLI. Keep exploring the Shopify CLI to further enhance your store management capabilities.

## Resources

- [Shopify CLI Documentation](https://shopify.dev/docs/apps/build/orders-fulfillment/order-management-apps/manage-test-orders)
- [Shopify Test Orders Documentation](https://help.shopify.com/en/partners/dashboard/managing-stores/test-orders-in-dev-stores)

---

**Maintained by [Kevin Horner]**
