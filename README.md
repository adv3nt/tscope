# tscope

## Requirements
* [Node.js](https://nodejs.org/)

## Setup
* clone and `cd` into repo
* `npm install`
* `cd ./config`
* You will need to [create a new Twitter app](https://apps.twitter.com/) to obtain the keys for `auth.json` in the next step. Fill in the **Name**, **Description** and **Website** fields with anything you want (Website does not have to be real), click Agree and Create app.
* Edit `auth.json` by filling in the keys from your new Twitter app
* Edit `config/queries.json` to include the query(s) you want to search for
* Edit `config/stasuses.json` to include the status(es) you want to reply with

## Usage
Search for default queries only:

	node tscope

Output usage information:

	node tscope -h

Search for 100 tweets using default queries:

	node tscope -c 100

Search for a custom query

	node tscope -q "paris+attacks+#isis"

Search for default queries and reply with default statuses:

	node tscope -r

Search for default queries and reply with a custom status:

	node tscope -r -s "we are the cure"

## Disclaimer
tscope is in experimental/early stages so use it at your own risk.
