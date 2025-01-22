# README

## Technical Test: Backend API Development with FastAPI

### Introduction
The objective of this technical test is to evaluate your skills in developing a backend API using FastAPI. The test should be completed within an estimated 4 hours.

### Requirements
1. **Develop an API** in Python using **FastAPI**.
2. The API must perform CRUD operations (Create, Read, Update, Delete) for a simple resource: **"Products"**.
3. The database can be either PostgreSQL or MySQL (participant's choice).
### Resource: Products
The **Product** resource should have the following model:
- `id`: Integer, primary key, auto-generated.
- `name`: String, required.
- `description`: String, optional.
- `price`: Decimal, required.
- `quantity`: Integer, required.
- `created_at`: DateTime, auto-generated when the product is created.

### Required Endpoints
1. **Create a Product**
   - **POST** `/products`
   - Accepts an object containing the product data (excluding `id` and `created_at`).
   - Returns the created product.

2. **Get All Products**
   - **GET** `/products`
   - Returns a list of products with pagination support (`skip` and `limit` as query parameters).

3. **Get a Product by ID**
   - **GET** `/products/{product_id}`
   - Returns the product corresponding to the specified `id`.

4. **Update a Product**
   - **PUT** `/products/{product_id}`
   - Updates the data of an existing product.
   - Returns the updated product.

5. **Delete a Product**
   - **DELETE** `/products/{product_id}`
   - Deletes the product corresponding to the specified `id`.
   - Returns a confirmation message.

### Additional Requirements (Optional but Appreciated)
We encourage you to include these extras if time permits:
- Configure model validations (e.g., positive prices).
- Unit tests using **pytest**.
- Implement basic pagination and filtering in the product listing.
- Configure CORS support.
- Include a **Docker Compose** file to launch the database along with the application.
- Create a **Makefile** to simplify command execution.

***

### What are we looking for? What does this prove?
* Assumptions you make given limited requirements
* Technology and design choices
* Identify areas of your strengths
* This is not a pass or fail test, this will serve as a common ground that we can deep dive together into specific issues
* Write code as if you are writing code in a team for a production app. Treat it as if you are releasing it to the public.
* Finally, we take pride in the code we write so ensure that your code is well encapsulated and follows a consistent convention. 

***

### Questions

* How long did you spend writing the application?
* What part of the application are you most proud of?
* If you had more time what would you improve in the application?


### How to complete this challenge
* Fork this repo on GitHub
* Complete the design and code as defined to the best of your abilities
* Complete your work in your own github repo (public), named aitaca-backend-test
* The branch should be named "aitaca"
* Complete your work in your own github repo and send the results and the Questions to us at tech@aitaca.io
