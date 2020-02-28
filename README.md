# GreenDeck-App

It's an assignment provided by GreenDeck, which is a Flask app application to provide results to the below tasks:

  - NAP products where discount is greater than n%.
  - Count of NAP products from a particular brand and its average discount.
  - NAP products where they are selling at a price higher than any of the competition.
  - NAP products where they are selling at a price n% higher than a competitor X.

## Install required packages

Run the below command to install required packaged before running the app.

```
pip install -r requirements.txt
```

## Run App

Run the below command to run the app

```
py GreenDeck_App.py
```
## Steps to make request to the app
  - After running the app notedown the host and port running at for eg. 127.0.0.1:5000
  - Install [POSTMAN](https://www.postman.com/downloads/)
  - Set Headers as follows
    ```
    Key: Content-Type           Value: application/json
    ```
  - Choose Request type as POST and set the URL to 127.0.0.1:5000/filter
  - Click on Body and choose Raw. Make sure type is selected as JSON or application/json
  - Copy paste the sample query
    ```
    { "query_type": "expensive_list", "filters": [{ "operand1": "brand.name", "operator": "==", "operand2": "prada" }] }
    ```
  - Click on send to query the results.
  
## Live build

  - This app runs [here] (http://greendeck-app.herokuapp.com/)
  - To make a request using POSTMAN, use below link
    ```
    http://greendeck-app.herokuapp.com/filter
    ```

