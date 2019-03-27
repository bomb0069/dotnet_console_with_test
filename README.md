# dotnet_console_with_test

## Reference from dotnet Document
>https://docs.microsoft.com/en-us/dotnet/core/testing/unit-testing-with-dotnet-test

## Creating the dotnet Solution File
>dotnet new sln

## Creating folder for Library project
>mkdir PrimeService
>cd PrimeService/

## Create Class Library Project
>dotnet new classlib

## Create Class PrimeService in namespace Prime.Services
>ren Class1.cs PrimeService.cs

## Add the class library project to the solution
>dotnet sln add ./PrimeService/PrimeService.csproj

# Creat Unit Test Project 

## Creating folder for Unit Test project
>mkdir PrimeService.Tests
>cd PrimeService.Tests

>dotnet new xunit

## Add the PrimeService class library as another dependency to the project.
>dotnet add reference ../PrimeService/PrimeService.csproj

## Add the test project to the solution
>cd ..
>dotnet sln add ./PrimeService.Tests/PrimeService.Tests.csproj

