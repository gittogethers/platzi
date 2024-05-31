![299105186-ea4e2746-5558-401d-809e-7270787e0d94](https://github.com/gittogethers/platzi/assets/107881423/e89f79c9-2110-4d5a-8de5-854030b444e4)

# Platzi x New Relic x GitHub Edu June Challenge

## Overview
In this challenge, you'll gain an understanding of how observability helps software engineering teams to understand the health and performance of their systems—and see beyond not just what errors occur, but to know when and why.

Through hands-on exercises, you'll explore observability and will learn how these practices enable engineers to gain insights into the inner workings of their applications, diagnose issues effectively, and make informed decisions to enhance performance and reliability.

You will also use Copilot to help you find and resolve problems in the coding infrastructure. Making you a more effective engineer.

## Using New Relic for Debugging
We'll be viewing the telemetry data we receive from the Astro Shop application on New Relic, an all-in-one observability platform that allows us to view telemetry data from different services and infrastructure.

## The Application
[Info about OTel and the app here]

## Using Copilot
GitHub Copilot is an AI coding assistant that helps you write code faster and with less effort, allowing you to focus more energy on problem solving and collaboration. Copilot offers coding suggestions as you type: sometimes the completion of the current line, sometimes a whole new block of code. You can accept all, or part, of a suggestion, or you can ignore the suggestion and keep typing. For this challenge, we encourage you to use Copilot to help you find errors in the code so you can better understand how to resolve them.

## The Task
I'm looking to purchase some items and have them delivered in time for the next meteor shower this year so I can see all of the shooting stars! However, as I navigate the application, I am noticing that special deals are not being applied to select items, and I am not getting the correct total as I go to complete my purchase. I want to use New Relic and view the data that is coming in from the application so I can fix the bugs and have my order shipped.

Step 1: Choose any 2 items from the Astro Shop and add them to your cart. For your second item, add multiple quantities of the items.
<img width="817" alt="Screenshot 2024-05-31 at 4 27 23 PM" src="https://github.com/gittogethers/platzi/assets/107881423/18a08c4b-f0f5-4dc4-9104-ece45180092a">

Step 2: Scroll to the bottom of the page, you should see an add for a discount off of one item. Click on the ad and then add that item to your cart.
<img width="800" alt="Screenshot 2024-05-31 at 4 27 31 PM" src="https://github.com/gittogethers/platzi/assets/107881423/085fcc62-67d7-4097-aa2f-f1ba7c6c1cc3">

Step 3: Enter in shipping and billing information and click Place Order.
<img width="801" alt="Screenshot 2024-05-31 at 4 27 38 PM" src="https://github.com/gittogethers/platzi/assets/107881423/069769b8-8ed7-4ed0-a3ca-d9acb23adec2">

Step 4: In your New Relic account, you should see a list of 17 services with `opentelemetry` listed as the provider. This is how you know you've instrumented your application with New Relic correctly.

[screenshot]

If you don't see this data appear in your New Relic account within a few minutes, review the setup instructions.

## Scenarios to solve for using Copilot:
Shipping was not properly calculated
Prices for multiple quantities of an item is not updating correctly
Incorrect CVV
Connected services
Ads for discounts


# Resources
- Get Started with New Relic - https://docs.newrelic.com/docs/new-relic-solutions/get-started/intro-new-relic/
- Getting Started with APM - https://docs.newrelic.com/docs/apm/new-relic-apm/getting-started/introduction-apm/
- Introduction to OpenTelemetry with New Relic-
https://docs.newrelic.com/docs/more-integrations/open-source-telemetry-integrations/opentelemetry/opentelemetry-introduction/

## New Relic for Students
https://newrelic.com/students

## Platzi Resources
- Git & Github -https://platzi.com/cursos/git-github/ 
- Github Copilot course https://platzi.com/cursos/github-copilot/ 
- New Relic - https://platzi.com/ruta/observability/ 

## Setup Instructions
New Relic Setup
- First, create your free New Relic account here.
- Get access to additional data and ingest through New Relic for Students.
- If you are currently verified through GitHub Education as a current student, log into your account and go to Help > Resources > New Relic for Students > Manage Account Eligibility > GitHub Education to allow New Relic to verify your student status. The additional data and ingest will be automatically added to your account.
- If you're not currently registered as a GitHub Education student, please go [here](https://education.github.com/discount_requests/application?utm_source=2024-06-11-Platzi-Challenge) to sign up. Once you've been successfully verified as a student, you'll be able to follow the steps above to receive the additional benefits.

Note that you can still participate in the challenge if you are not verified as a GitHub Education student

- Fork this repository! (Please do not clone)
- Click on Code, then Create Codespace on main
- Add your New Relic license key to your application
- In your New Relic account, click on your name, then click on API Keys
- Under Type, find the key that says `INGEST - LICENSE`, click on the three dots at the end of the row, and click `Copy key`
- Paste your New Relic license key in the `otel-config-extras.yml` file under exporters: api key
- Paste the license key again in the .env file in place of `${NEWRELIC_LICENSE_KEY}`


## GitHub Copilot Setup
Subscription to Copilot. To use GitHub Copilot in Visual Studio Code, you must have an active GitHub Copilot subscription. For information about how to get access to Copilot, see "About GitHub Copilot."
Visual Studio Code. To use GitHub Copilot in Visual Studio Code, you must have Visual Studio Code installed. For more information, see the Visual Studio Code download page.
Copilot extension for Visual Studio Code. To use GitHub Copilot in Visual Studio Code, you must install the GitHub Copilot extension. For more information, see "Set up GitHub Copilot in Visual Studio Code" in the Visual Studio Code documentation.


You're ready to run your application!
Running the application

Run the `make start` command.
Stopping the application
Exit the Codespace


