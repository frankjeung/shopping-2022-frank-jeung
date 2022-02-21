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

Recieved help from https://github.com/prof-rossetti/intro-to-python/blob/main/notes/python/packages/sendgrid.md#email-templates 
