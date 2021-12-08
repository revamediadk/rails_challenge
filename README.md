# rails_challenge

This project is part of the job interview for joining Rentola's core development team.

We are heavily using Ruby on Rails (6/7) in Rentola in multiple projects and thus we are providing the following challenge and you will need to implement a solution for it.

You goal is to be able to:

1. Implement a working solution as per the provided requirements.
2. Make sure your code is clean and modular (SOLID/DRY).
3. Write sample tests for parts of your code.
4. Instructions on how to setup the environment and run the project.

Bonus points for:

1. Implement a dockerfile.
2. Lint your code using Rubocop or alike.
3. Write a Github action to run the tests or/and Rubocop.
4. Deploy to Heroku or alike.

## Challenge Requirements

Implement a RoR API endpoint `/calculate` to:
1. Receive a form submission with two numbers A and B and an operation (`SUM`, `SUB`, `TIMES`, or `DIVIDE`).
2. It should return 200 response with the result of the operation.

Example:

```
curl -X POST 'http://localhost:3000/calculate' \
--form 'A="100"' \
--form 'B="50"' \
--form 'OPERATION="SUM"'
```

Response:

```
{
  "result": 150
}
```
