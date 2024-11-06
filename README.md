# Etsy Product Uploader

This repository provides a simple script to upload products to an Etsy shop using the Etsy API. The script is designed as a starting point for integrating with Etsy’s platform for automated product management.

## Features
- Connects to Etsy’s API to create new product listings.
- Demonstrates basic usage of the Etsy API for product upload.
- Accepts product details like title, description, price, quantity, tags, and materials.

## Prerequisites
1. **Python 3.x**: Ensure you have Python installed.
2. **Requests Library**: Install the requests library for handling HTTP requests.

   ```bash
   pip install requests
   
3. Etsy API Key and OAuth2 Access Token:
- Register your application on Etsy to obtain an API key.
- Complete the OAuth2 authorization process to get an access token.

## Setup
1. Clone the repository:
git clone https://github.com/yourusername/etsy-product-uploader.git
2. Navigate to the project directory:
cd etsy-product-uploader
3. Replace placeholders in the script with your API key, Shop ID, and OAuth2 access token.

## Usage
To upload a product to your Etsy shop, modify the upload_product_to_etsy function in etsy_uploader.py with product details:
upload_product_to_etsy(
    title="Sample Product",
    description="This is a sample product description.",
    price=25.99,
    quantity=10,
    tags=["sample", "handmade"],
    materials=["cotton", "wood"]
)

Then run the script:
python etsy_uploader.py

If successful, the product will be uploaded to your Etsy shop.

## Troubleshooting
-401 Unauthorized: Check if your access token is valid and your API key is correct.
-403 Forbidden: Ensure your Etsy API application has permissions for listing creation.
