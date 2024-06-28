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

### Type in terminal 
    dotnet run

## Saving the data in a databse
1. NuGet packages must be added to support the database and diagnostics used in this tutorial. Type in Terminal:

```dotnet add package Microsoft.EntityFrameworkCore.InMemory```

```dotnet add package Microsoft.AspNetCore.Diagnostics.EntityFrameworkCore```

For more information, see:
https://learn.microsoft.com/en-ca/aspnet/core/tutorials/min-web-api?view=aspnetcore-8.0&tabs=visual-studio-code#add-nuget-packages
