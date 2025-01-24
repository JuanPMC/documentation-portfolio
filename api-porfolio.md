# Technical documentation for api-portfolio
Is the microservice that holds most of the backend activities for project Portfolio.
## Logic Endpoints:
- Get the value of a stock: 
    - Endpoint: ```/value/<ticker_id>``` 
- Buy a stock:
    - Endpoint: ```/buy/<ticker_id>/<ammount>```
- Sell a stock:
    - Endpoint: ```/sell/<ticker_id>```
- Get the portfolio information:
    - Endpoint: ```/portfolio```
- Get the montly ranking:
    - Endpoint: ```/ranking```
## Authentication:
Authentication must be done using googles oauth.
### New auth endpoint:
- Redirect user to Google's OAuth 2.0 authorization endpoint
    - Endpoint: ```/auth/login```
- Handle the callback from Google after user authentication
    - Endpoint: ```/auth/callback```