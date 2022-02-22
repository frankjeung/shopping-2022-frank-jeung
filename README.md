# shopping-2022-frank-jeung

[Project Description] (https://github.com/prof-rossetti/intro-to-python/blob/main/projects/shopping-cart/README.md)

## Installation

Clone or download from [GitHub source] (https://github.com/prof-rossetti/intro-to-python/blob/main/projects/shopping-cart/README.md), then navigate into the project repositor:

## Usage

Run the program:

```sh
python shopping_cart.py
```

Received help from https://www.youtube.com/watch?v=3BaGb-1cIr0 

# IF USING THIRD-PARTY PACKAGES, USE A NEW ENV:
conda create -n shopping-env python=3.8 
conda activate shopping-env
pip install -r requirements.txt # (after specifying desired packages inside)

Received help from Clyde Leef

# Instructions for how obtaining your credentials and setting up a local ".env" file. 
First, you should sign up for a SendGrid account, then follow the instructions to complete your "Single Sender Verification", clicking the link in a confirmation email to verify your account.

Second, you should create a SendGrid API Key with "full access" permissions. You want to store the API Key value in an environment variable called SENDGRID_API_KEY.

Third, you should set an environment variable called SENDER_ADDRESS to be the same email address as the single sender address you just associated with your SendGrid account.

Fourth, you should create an ".env" file that contains all of these environment variables.

Laslty, you could use the sample HTML and test data to specifiy the structure of all emails

Sample HTML
     <img src="https://www.shareicon.net/data/128x128/2016/05/04/759867_food_512x512.png">

    <h3>Hello this is your receipt</h3>

    <p>Date: {{human_friendly_timestamp}}</p>

    <ul>
    {{#each products}}
	    <li>You ordered: ... {{this.name}}</li>
    {{/each}}
    </ul>

    <p>Total: {{total_price_usd}}</p>

Sample Test Data
    {
        "total_price_usd": "$99.99",
        "human_friendly_timestamp": "July 4th, 2099 10:00 AM",
        "products":[
            {"id": 100, "name": "Product 100"},
            {"id": 200, "name": "Product 200"},
            {"id": 300, "name": "Product 300"},
            {"id": 200, "name": "Product 200"},
            {"id": 100, "name": "Product 100"}
        ]    
    }


Recieved help from https://github.com/prof-rossetti/intro-to-python/blob/main/notes/python/packages/sendgrid.md#email-templates 
