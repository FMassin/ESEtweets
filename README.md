# ESE tweets

```bash
> pip install -r requirements.txt
> export 'CONSUMER_KEY'=' your key ' 
> export 'CONSUMER_SECRET'=' your secret '
> python ESEtweets.py 
Please go here and authorize: https://api.twitter.com/oauth/authorize?oauth_token=..
Paste the PIN here:
```

After completing authorization, the content of file `./tweet.json` (in current workspace) will scanned continuously, and when it is updated, its content will be sent as a tweet and file will archived (renamed). An example `tweet.json` might be given by:

```bash
echo '{"text": "Hello world!"}' >  ./tweet.json
```