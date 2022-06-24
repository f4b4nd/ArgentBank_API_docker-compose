# Project #10 - Argent Bank API

This codebase contains the code needed to run the backend for Argent Bank.

## 1.Prerequisites :
- Docker
- Docker-compose

## 2. Installation

You can clone this repository with the following command :

`git clone https://github.com/f4b4nd/ArgentBank_API_docker-compose.git`


## 3. Launch backend + MongoDB
- Get into the folder : `cd ./ArgentBank_API_docker-compose/`
- Run the commmand : `docker-compose up`

Your server should now be running at http://locahost:3001

---

## 4. Add Data to MongoDB via backend
- After running `docker-compose up`, you should have 2 containers running: `bank-api` and `bank-mongodb`
- Open backend container via the following command : `docker exec -it bank-api /bin/sh`
- Inside the container, run the following command: `npm run populate-db`

### Populated Database Data

Once you run the `populate-db` script, you should have two users in your database:

### Tony Stark

- First Name: `Tony`
- Last Name: `Stark`
- Email: `tony@stark.com`
- Password: `password123`

### Steve Rogers

- First Name: `Steve`,
- Last Name: `Rogers`,
- Email: `steve@rogers.com`,
- Password: `password456`

## 5. API Documentation

To learn more about how the API works, once you have started your local environment, you can visit: http://localhost:3001/api-docs

---
## Design Assets

Static HTML and CSS has been created for most of the site and is located in: `/designs`.

For some of the dynamic features, like toggling user editing, there is a mock-up for it in `/designs/wireframes/edit-user-name.png`.

And for the API model that you will be proposing for transactitons, the wireframe can be found in `/designs/wireframes/transactions.png`.
