# trello-api-test
Smoke test for testing Trello API with Postman.
## General info
In this test by abstracting low-level commands, and by structuring request formation you will be able to create a board, crate a list and cards in your board, also you will be able to move card from one list to another, invite a member, and delete all parts of board(cards, lists), and at the end of collection you can delete a board. 
## Prerequisites
Log in to Trello https://trello.com/en and visit https://trello.com/app-key to get a <em>key</em> and <em>secret</em>, for <em>token</em> you must visit https://trello.com/1/token/approve and get it. These need to be supplied if you want to run collection in Postman or using newman.
When you get your <em>key</em> and <em>secret</em>, go to environment and replace initial and current value with yours <em>key</em> and <em>secret</em>, also replace {{dummyToken}} with your <em>Token</em>.<br />
For variable email you must replace dummy_email@gmail.com with email address from the member you want to invite to a board. 
## Postman installation
Postman is a lightweight tool the interact with Web Services. For download Postman application go to https://www.postman.com/downloads/ 
## Newman installation
For Newman installation, first you must be ensure that you have Node.js >= v10. <a href ="https://nodejs.org/en/download/package-manager/">Install Node.js via package manager.</a> <br />
The easiest way to install Newman is using NPM.
For install newman globally on your system, run `$ npm install -g newman`
## Usage 
 After you export your Postman Collection as a json file from the Postman App, you can run it using Newman with <br />
 `$ newman run trellotestcollection.json`

