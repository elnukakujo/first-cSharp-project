# My first CSharp environment

## Description
The purpose of this environment is for me to learn how to use C# and .Net, as well as what they offer.

## Installation of C# and .Net

1. Install VSCode
2. Install the C# Dev Kit
3. ```sudo apt-get install -y dotnet-sdk-8.0 ```

## Creation of a C# project

1. Create a folder/github repo where you want your project to be
2. Using cmd go to that folder in the terminal
3. Create the project using:
    ```dotnet new {typeOfApp} -n {appName}```
4. ```cd {appName}```

### Types of app

See https://learn.microsoft.com/en-us/dotnet/framework/get-started/overview#net-framework-class-library

## Run the app

    dotnet run

#### (Following is not necessary for this project)

## Saving the data in a database
1. Packages must be added.
```
dotnet add package Microsoft.EntityFrameworkCore.InMemory
dotnet add package Microsoft.AspNetCore.Diagnostics.EntityFrameworkCore
dotnet add package NSwag.AspNetCore
dotnet add package Microsoft.EntityFrameworkCore.Sqlite
dotnet add package Microsoft.EntityFrameworkCore.Design
```
2. Add to appsettings.json
```
"ConnectionStrings": {
    "BookLibraryConnection": "Data Source=booklibrary.db"
  }
```
3. Create and apply the migrations
```
dotnet tool install --global dotnet-ef
dotnet ef migrations add InitialCreate
dotnet ef database update
```
4. More modifications middleware needs to be applied. For an example of a functionning code, see:
https://github.com/elnukakujo/Book-Library-Management-API

For more information, see:
https://learn.microsoft.com/en-ca/aspnet/core/tutorials/min-web-api?view=aspnetcore-8.0&tabs=visual-studio-code#add-nuget-packages
