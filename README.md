# ShopyStoreV2


# A simple, cross platform, modularized ecommerce system built on .NET Core 



## Docker

For testing purpose only `docker run -p 5000:80 simplcommerce/ci-build`



## Visual Studio 2017 and SQL Server

#### Prerequisites

- SQL Server
- [Visual Studio 2017 version >= 15.8 with .NET Core SDK 2.2.101](https://www.microsoft.com/net/download/all)

#### Steps to run

- Update the connection string in appsettings.json in SimplCommerce.WebHost
- Build whole solution.
- In Solution Explorer, make sure that SimplCommerce.WebHost is selected as the Startup Project
- Open Package Manager Console Window and make sure that SimplCommerce.WebHost is selected as Default project. Then type "Update-Database" then press "Enter". This action will create database schema.
- In Visual Studio, press "Control + F5".
- The back-office can access via /Admin using the new user account

## Mac/Linux with PostgreSQL

#### Prerequisite

- PostgreSQL
- [.NET Core SDK 2.2.101](https://www.microsoft.com/net/download/all)

#### Steps to run

- Update the connection string in appsettings.json in SimplCommerce.WebHost.
- Run file simpl-build.sh by "sudo ./simpl-build.sh". For ubuntu 18 "sudo bash simpl-build.sh"
- In the terminal, navigate to the "src/SimplCommerce.WebHost" type "dotnet run" and hit "Enter".
- Open browser, open http://localhost:5000. The back-office can access via /Admin using the new user account.

## Technologies and frameworks used:

- ASP.NET MVC Core 2.2
- Entity Framework Core 2.2
- ASP.NET Identity Core 2.2
- Angular 1.6.3
- MediatR 6.0.0 for domain event



## How to contribute

- Star this project on GitHub.
- Report bugs or suggest features by create new issues or add comments to issues
- Submit pull requests
- Donate us


