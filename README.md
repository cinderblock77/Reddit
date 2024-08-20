# Reddicator
This Python script allows you to wipe your Reddit history. It replaces each comment and post with random text before deleting them.

## Installation
1. Git clone this repository: `git clone https://github.com/Jelly-Pudding/ereddicator.git`
2. Install this specific version of PRAW (Python Reddit API Wrapper):
`pip install praw==7.7.1`

## Instructions
1. Obtain a `client_id` and `client_secret`:
- Go to https://www.reddit.com/prefs/apps
- Click "Create App" or "Create Another App"
- Choose "script" for personal use
- Fill in any name and for the redirect uri put http://localhost:8080
- After creation, the client_id is the string under "personal use script"
- The client_secret is labeled "secret"
2. Create a file named `reddit_credentials.ini` in the same directory as the script.
3. Add your Reddit API credentials to the file in the following format:
    ```
    [reddit]
    client_id = YOUR_CLIENT_ID
    client_secret = YOUR_CLIENT_SECRET
    username = YOUR_USERNAME
    password = YOUR_PASSWORD
    ```
4. Run the script using Python: `python ereddicator.py`.