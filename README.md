# Polling system API

This API functions as a backend system designed to perform various actions related to polling:

-Question Creation: Enables the creation of new questions.
-Option Addition: Allows the addition of options to specific questions.
-Voting on Options: Permits users to vote on available options.
-Deletion Capabilities: Supports the deletion of both questions and options.
-Comprehensive Question Viewing: Provides a view of questions alongside all associated options.

## Polling system Features

- Create questions
- Add options to question
- Delete a question
- Delete an option
- Add vote to an option
- View a question with all of its options

## Installation Guide

- Clone this repository.
- Run npm install to install all the dependencies.
- Create an .env file in your project root folder and add your variables.

## Usage

- Run node index.js to run the application.
- Connect to the API using Postman on port 8000.

## API Endpoints

| HTTP Verbs | Endpoints                          | Action                                 |
| ---------- | -----------------------------------| -------------------------------------- |
| POST       | /questions/create                  | To create a  question                  |
| POST       | /questions/:id/options/create      | To add options to a specific question  |
| DELETE     | /questions/:id/delete              | To delete a question                   |
| DELETE     | /options/:id/delete                | To delete an option                    |
| PUT        | /options/:id/add_vote              | To increase the count of votes         |
| GET        | /questions/:id                     | To view a question and its options     |

## Tech stack
* NodeJS
* ExpressJS
* MongoDB
* Mongoose ODM
