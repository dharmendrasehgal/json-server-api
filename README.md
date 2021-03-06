# json-server-api
First, let's install json-server in our system using the following command:

`$ npm install -g json-server`

Next, create a folder for your server and create a JSON file (data.json) with the following content:

`{
    "users":[
        {
            "id": 1,
            "first_name": "Robert",
            "last_name": "Schwartz",
            "email": "admin@email.com"
        }

    ],
    "accounts": [
        {
            "id": 1,
            "name": "",
            "email":"",
            "phone": "",
            "industry": "",
            "website": "",
            "description": "",
            "createdBy": 1,
            "createdAt": "",
            "isActive": true
        }
    ],
    "contacts": [
        {
            "id": 1,
            "first_name": "",
            "last_name": "",
            "account": 1,
            "status":1,
            "source": 1,
            "email": "",
            "phone": "",
            "address": "",
            "description": "",
            "createdBy": 1,
            "createdAt": "",
            "isActive": true
        }
    ],
    "activities": [
        {
            "id": 1,
            "description": "",
            "createdAt" : "",
            "contact": 1,
            "status": 1
        }
    ],
    "contactsources": [
        {
            "id":1,
            "source": ""
        }
    ],
    "contactstatuses": [
        {
            "id":1,
            "status": ""
        }
    ],
    "activitystatuses":[
        {
            "id":1,
            "status": ""
        }
    ]
}`

We added empty entries for JSON data. Feel free to add your own data or use a tool like Faker.js to automatically generate fake data.

Next, you need to start the JSON server using:

`$ json-server --watch data.json `

Your REST API server will be running at http://localhost:3000.

We'll have the following resources exposed:

http://localhost:3000/users
http://localhost:3000/accounts
http://localhost:3000/contacts
http://localhost:3000/activities
http://localhost:3000/contactsources
http://localhost:3000/contactstatuses
http://localhost:3000/activitystatuses
