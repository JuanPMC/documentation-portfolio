# Documentation for the Porfolio project
It's a platform to test investment strategies by competing with your friends. I pulls real stock data to produce wins and loses, it computs mothly winners, uses google oicd, hosted in aws. Written in fast-api to lower costs, improve efficiency and speed.
## Project use cases:
### 1. Allows for mutiple users to have separate portfolios
    Use a secure multi user application, this means porfolio information must be stored as per user bases.
### 2. Uses real-time stock market information
    Must connect to api endpoints to gather real time accurate information about stock prices.
### 3. Allows users to buy stocks
    Users must be able to transform cash(1000$ initial value) into stocks, at market price.
### 4. Allows users to sell stocks
    Users must be able to transform stocks into cash at market price.
### 4. Allows playets to compair their performance with others
    Players must be able to see a ranking of them and other users.
## Architecture of the project
- The aplication backend is hosted in api-portfolio(AWS fargate)
- The frontend is hosted in an app called front-portfolio(S3 bucket)
- Database will be hosted outside of AWS
- Rankings will be computed monthly in aws fargate (for the future)