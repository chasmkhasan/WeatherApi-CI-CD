# WeatherApi
We are going to do a team project where we build a Weather API using Minimal API in C# and a client with React using Vite.
We will use Test Driven Development process to create this application and will be deploying a CI/CD pipeline.

## Structure of Project:
|   Tasks     |   Framwork    |  Effect  |
|-----|--------|-------|
|C# |  Minimal API   | Out via Swagger
|JS |   React, React-Dom, Vite   | Fetching Data via Endpoints
|Database |   InMemory   | InMemmory has limmited dat
|Model | VS C# & .NET Core 6   | Get and Post
|Connection |  JSON   |  Global Datbase
|TDD |  XUnit Test   | Red-Green-Refactor

## XUnit Test: We have taken one endpoint with 3 tests:
a) GetStatistics_ReturnsFormattedCountString(), b) IncrementAPICall_IncrementsCount(), c) GetStatistice_Return()
An ApiCallCount test purpose of checking the increment method and getting statistics method even though I have taken a variable with parameter Finally I have returned apiCallCount.

Now I will test my code and create some method which is not connected with my real test.
Since I have created an “IncrementAPICall_IncrementsCount” method, let's start to test. In the Arrange side I have taken a variable  where I have declared one object to carry forward of ACT. ACT side I have called “IncrementAPICallAsync”. In the Assert part I have mentioned 1 and Arrange side I have put initialCount = 0, Since this test is purpose of checking the increment. “GetStatistics_ReturnsFormattedCountString” side I have tested in is the same but the value equation will be the same because of its “GetStatistics_ReturnsFormattedCountString”.

Real test “GetStatistice_Return()” below which is connected to our weatherAPICall.

Write a Test: First I need to understand the behaviour of Code. The Statistics API will count how many users have been hit on the rest of the API. The main behaviours are increment and count. 

Run the Test: Since I am just assuming the behaviour I need to check is it going to fail or pass. Failure is a positive sign for a test. 

Write the Code: Now I have connected with my endpoint since its connection with HTTP client that is why I have declared some class and class has been inherited with iRepository. I have also declared a constructor and have also declared some variables. The ACT side I have called endpoint and Assert side I have declared one object which will carry forward or fetch the data and cross check with the endpoint.

Run All The Test: We need to do a clean solution and build a solution so we will get one project without error. Then click run all tests. If it's passed so it is positive. I was crossing my fingers.

Refactors: This part is very important for understanding the code. I have focused on humans who can read my code because machines can read any massy code.


## Team

- [Reza](https://github.com/Rezaeskandar)
- [Md. Kamrul Hasan](https://github.com/chasmkhasan)
- [Md Ruhul Amin](https://github.com/Md-Ruhul-Amin-Rony)
- [Tasmia Zahin](https://github.com/tasmiazahin)
- [Suhagan Mostahid](https://github.com/suhagan)
- [Abdirahman Farah](https://github.com/Abfar90)
