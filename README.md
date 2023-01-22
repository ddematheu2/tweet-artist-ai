# Tweet Artist AI

This repo provides the code to create a bot that listens for mentions on Twitter and illustrates the Tweet to which the mention is a reply to. The bot uses the Tweepy library to interact with the Twitter APIs to get tweet information and post tweet on behalf of the bot. It uses the Open AI library to interact with Open AI [Dall-E](https://beta.openai.com/docs/guides/images) model to generate images.

## Running Locally

### Pre-Reqs

1. Create a Twitter account where you want your bot to connect to. Can be an existing account or new one. You will use this account to have the bot use to respond to tweets as as for your developer account below.
2. Have a [Twitter developer account](https://developer.twitter.com/en). You will need get the necessary auth tokens for the account to enable the bot. This includes:
   - Read and write permissions for which you will need to configure your application within the Twitter developer portal.
   - Access to the Twitter v1.1 APIs to access media upload. This access is granted by accessing elevated status. (Simple form you can submit after creating the account.)

3. Have an [Open AI developer account](https://openai.com/api/). You get some free credits by default. From here you will need an auth secret to enable your bot.
4. Install [Python 3.9 (or later)](https://www.python.org/downloads/)
5. Pip install dependencies including:
   - [tweepy](https://docs.tweepy.org/en/stable/getting_started.html)
   - [openai](https://beta.openai.com/docs/libraries)

### Run

1. Clone this repo into your machine.
2. Go to the file, an update the values for all the auth tokens for Twitter and Open AI, also make sure to update the handle that you want the bot to be listening for.
3. In your command prompt, navigate to the folder where the repo was cloned
4. Run the script

    ``` bash
    
        python twitterArtist.py
    
    ```

5. Navigate to Twitter and try mentioning your bot as a reply to a tweet you want to illustrate.
