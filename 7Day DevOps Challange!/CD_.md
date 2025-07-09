# What is CI/CD?

Let's understand CI/CD by starting with something familiar - cooking!
In traditional cooking, there are chefs (developers) that come up with new recipes, and restaurant staff (operations) that follow the recipes and serve the dishes to customers (users).

## Things can go wrong when the chef releases a new recipe (i.e. new code):
- 😦 The restaurant's pantry doesn't have the ingredients for the new recipe.
- 😨 Some restaurant staff are still cooking with the old recipe.
- 😰 The new recipe comes with special serving instructions that servers don't know about, so customers aren't getting the full experience.

If there was CI/CD for cooking...

Now, let's imagine if there was a way to apply some automations to this process:
- The pantry automatically stocks all the required ingredients for the latest recipes.
- Cooking equipment automatically cooks identical, consistent dishes based on the latest recipe.
- Servers automatically know about the new serving instructions, and serve dishes to customers without any delays.
- A restaurant manager automatically checks that everyone is following the instructions for the latest recipe of every dish.

These automations make the flow from the chef's latest recipe to the customer's plate much more efficient and reliable!

## In software development, CI/CD works similarly

The goal of CI/CD is to make the flow from code changes to a live application as efficient and reliable as possible. To do this, automations are set up across the software development and deployment process.
- In project 1 of this challenge, you'll start by setting up a Development environment i.e. the test kitchen where developers write code.
- In project 2, you'll connect your development environment to GitHub i.e. the recipe book storing different versions of the code.
- In project 3, you'll store dependencies in CodeArtifact i.e. the pantry for pre-built code your app needs to function.
- In project 4, you'll build your code with CodeBuild i.e. the cooking process that prepares code for deployment.
- In project 5, you'll use CodeDeploy to deploy your code to a Web server/Live application i.e. servers that deliver code to users.
- In project 6, we'll do a bonus project to learn how to use CloudFormation to turn your infrastructure into code.
- Finally, in project 7, you'll set up the CI/CD pipeline with CodePipeline i.e. the restaurant manager that makes sure code is automatically flowing from one stage to the next.
