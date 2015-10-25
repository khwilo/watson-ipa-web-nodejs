## Watson Intelligent Personal Assistant (Web Demo)
According to Wikipeida, "an [intelligent personal assistant](https://en.wikipedia.org/wiki/Intelligent_personal_assistant) is a software agent that can perform tasks or services for an individual."  In this demo, we'll combine two Watson services to illustrate the basics of intelligent task performance:

1. Capture user input.
2. Classify this input into one of several supported tasks
3. Ask user for any additional information required to complete the task
4. Execute the task for the user (an exercise left for you to complete)

These are the tasks we'll attempt to classify:

* Schedule a meeting
* Send an email
* Set an alarm
* Numeric calculations
* Map directions
* Location recommendations
* Off-topic
* Unknown

![https://bluemix.net/deploy?repository=https://github.com/biosopher/watson-ipa-web-nodejs](https://github.com/biosopher/watson-ipa-web/blob/master/wiki/media/deploy_to_bluemix.png)

### Getting to know the two Watson Services
To act on our user's intent, we first need to classify it into one of our categories above.  The [Watson Natural Language Classifier service](https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/doc/nl-classifier/) uses deep machine learning techniques to return the top matching predefined classes for short text inputs.  We'll train the NLC using various text examples of users making the requests above.  Next, we'll need to ensure we have all the information required to complete the user's request.  To do this, we'll rely on the [Watson Dialog service](http://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/dialog.html) which supports building conversations between a user and an application. The Dialog service will track and store information obtained during the conversation until we have all the additional information required to complete the task. 

The following sections in the wiki will guide you through these tasks:

* Setting up a Bluemix account
* Start the Natural Language Classifier service on Bluemix
* Train the Natural Language Classifier service
* Start the Dialog service on Bluemix
* Configure your Dialog service with IBM's Dialog XML
* Connect the NodeJS app to your Natural Language Classifier service
* Connect the NodeJS app to your Dialog service

