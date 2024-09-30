# Trello-API-Automation-Testing
This repository contains automation testing for Trello API endpoints using Postman. The goal of this project is to automate and validate various Trello API functions such as creating boards, managing lists, and cards.

## Project Overview
The Trello API allows users to manage boards, lists, and cards programmatically. This project focuses on automating the testing of key endpoints related to board and task management.

## Key Automated API Tests:
Create Board: Automatically test the creation of a new board.
Get Board Details: Validate fetching details of a single board.
Create TO DO List: Automate adding a new list to a board.
Move Card: Ensure cards can be moved between lists.
Delete Card: Verify that cards can be deleted.
Automated API Endpoints
The following endpoints are automated and tested:

POST /1/boards/: Create a new board.
GET /1/boards/{board_id}: Get details of a specific board.
POST /1/boards/{board_id}/lists: Create a TO DO list on a board.
POST /1/cards: Create a new card in the TO DO list.
PUT /1/cards/{card_id}: Move card to another list.
DELETE /1/cards/{card_id}: Delete a card.

## Tools Used
Postman: For writing, automating, and running API tests.
Newman: Used to run the Postman collection in CI/CD pipelines.
GitHub: For version control and project repository.

## How to Use
1. Clone the repository:

git clone https://github.com/yourusername/Trello-API-Automation-Testing.git

2. Install Newman:
   
npm install -g newman

3. Run the Postman collection with Newman:

newman run TrelloAPIInitialCollection.json

## Postman Collection
The Postman collection used for automating these tests can be found in the repository as TrelloAPIInitialCollection.json. You can import this file into Postman for further testing and editing.

## Test Coverage
Automated tests for creating and managing Trello boards, lists, and cards.
Covers CRUD operations for boards and tasks.
Validation of request status codes, response data, and error handling.
