# Lettuce-BrowserStack

A sample to run lettuce over BrowserStack Automate.

### Install dependencies

Navigate to appropriate directory for testing and then install the dependencies by running

`pip install -r requirements.txt`

### BrowserStack Authentication

Export the environment variables for the username and access key of your BrowserStack account.
These can be found on the automate accounts page on [BrowserStack](https://www.browserstack.com/accounts/automate)

`export BROWSERSTACK_USERNAME=<browserstack-username>`

`export BROWSERSTACK_KEY=<browserstack-access-key>`

### Run the tests

- To run series tests, run `lettuce`
- To run series tests with local, run `TEST_TYPE=local lettuce`
- To run tests for each feature, run `TEST_TYPE=parallel lettuce`
- To run tests for each feature with local, run `TEST_TYPE=parallel,local lettuce`

------

#### How to specify the capabilities

The [Code Generator](https://www.browserstack.com/automate/python#setting-os-and-browser) can come in very handy when specifying the capabilities especially for mobile devices.
