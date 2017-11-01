# T-Hawk

Simple Twitter bot that auto likes and retweets based on a configured hashtag. Use for a special event or conference (like a DevFest!) to help increase social engagement and awareness.

This project derives its name from a small drone (UAV) of the [same name](https://en.wikipedia.org/wiki/Honeywell_RQ-16_T-Hawk) with no other affiliation or association.

## Getting Started

* Log in and create a [Twitter app](https://apps.twitter.com/)
  * **NOTE:** Use the account you wish to like & retweet with (which most likely isn't your personal one)
  * **NOTE:** You do not need a Callback URL for this app
* Start a new Google Apps Script project by clicking on ["Start Scripting"](https://www.google.com/script/start/)
* Copy the code from [code.gs](https://github.com/neojato/T-Hawk/blob/master/code.gs) into the new file created for you
* Enter the appropriate Twitter keys you received from your new Twitter app in lines 3-6
* Enter your hashtag on line 7 (include "-RT" to exclude retweets from being liked and retweeted)
  * example: "#DevFest -RT"
* From the Apps Script menu, choose "Resources" and then "Libraries"
  * In the "Add a library" field, enter the following project key:
    * `11dB74uW9VLpgvy1Ax3eBZ8J7as0ZrGtx4BPw7RKK-JQXyAJHBx98pY-7`
  * Click the "Add" button
  * Change the "Identifier" field to `Twitter`
  * Change the "Version" to `22`
  * Click "Save"
* From the Apps Script menu, choose "Run" and then "Start_Bot"
* Create a trigger to continually monitor the hashtag
  * From the Apps Script menu, choose "Edit" and then "Current project's triggers"
  * Follow instructions to add a new trigger
  * Setup your trigger to match the following settings:
    * devfest_twitterBot
    * Time-driven
    * Hour timer
    * Every hour
* Enjoy!

## Contributing

This project is open for contributions, suggestions, and ideas. Feel free to submit a PR and/or create an [Issue](https://github.com/neojato/T-Hawk/issues) with bugs, suggestions, and ideas. Stars are always welcome too!

See [list of contributors](https://github.com/neojato/T-Hawk/graphs/contributors).

### License

Project is published under the [MIT license](https://github.com/neojato/T-Hawk/blob/master/LICENSE).  
Feel free to clone and modify repo as you want, but don't forget to add reference to original authors, thanks!

###### The T-Hawk Project is not endorsed and/or supported by Google, the corporation.
