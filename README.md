<img src="https://img.shields.io/badge/code%20style-black-000000.svg" align="right"/>

<img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" align="right"/>


# PyTweet

PyTweet is an api wrapper made for receiving info from twitter using twitter's api version 2! 

## Installation

### Windows
```bash
py3 -m pip install PyTweet
```
### Linux
```bash
python -m pip install PyTweet
```

## Usage

#### First we create our client instance using pytweet.Client()
```py
import pytweet

client=pytweet.Client("Your Bearer Token Here!!!", consumer_key="Your consumer_key here", consumer_key_secret="Your consumer_key_secret here", access_token="Your access_token here", access_token_secret="Your access_token_secret here") #if you dont have one make an application in https://apps.pytweet.com
```

#### After that we use functions to get info from twitter api.
```py
user=client.get_user_by_username("TheGenocides")
print(user.name, user.username, user.id)
#Return The user's name, username, and id

tweet=client.get_tweet(Tweet ID Here)
print(tweet.text, tweet.id, tweet.author.username)
# Return the tweet's text, id, and the author's username.
```

# Contribute
You can Contribute or open an issue regarding this wrapper [here](https://github.com/TheFarGG/PyTweet)! 

# Licence
[MIT](https://opensource.org/licenses/MIT)
