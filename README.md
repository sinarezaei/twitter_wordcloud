![alt text][pypi_version] ![alt text][licence_version]

# Twitter Wordcloud: word-cloud builder from tweets with RTL support

Tested with:
* Python 3.6+

Use the following command to install requirements using pip:
```
pip install -r requirements.py
```

## Twitter API
Open `twitter_wordcloud.py`, replace your credentials in TwitterApp constructor (line 24):

```python
app = TwitterApp(
    api_key='YOUR_API_KEY',
    api_secret_key='YOUR_API_SECRET_KEY',
    app_name='YOUR_APP_NAME',
    bearer_token='YOUR_BEARER_TOKEN'
)
```

## Usage example

Run `twitter_wordcloud.py` or use `create_word_cloud` method to create word-clouds.
```python
from twitter_wordclould import create_word_cloud

create_word_cloud('YOUR_TWITTER_USERNAME', target_tweet_count=3200, filename='output.png')
```
