# Payments-with-Stripe

A Python (Flask) app that interacts with the Stripe API (REST API) for accepting credit card payments. Users are identified by unique email addresses. New users are saved in a local MongoDB database and recurring charges can be made for saved users (only need to store the user email and Stripe ID for that customer). Postman used for testing API calls.

How to Get Started
Install all the necessary packages (best done inside of a virtual environment)
pip install -r requirements.txt

Make sure 'mongod' is installed and running - http://docs.mongodb.org/manual/installation/

Get your Stripe API keys (https://manage.stripe.com/account/apikeys) and add PUBLISHABLE_KEY and SECRET_KEY to your ~/.bashrc file

export PUBLISHABLE_KEY=<your_publishable_key_from_stripe> 
export SECRET_KEY=<your_secret_key_from_stripe>
and reload

. ~/.bashrc

Run the app
python app.py
