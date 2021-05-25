# Eau Claire's Salon

By James Wyn

## Description
This MVC web app will allow the user to add Stylists and Clients to a database as well as displaying the information.

## Technologies Used

* C#
* ASP.NET Core
* Entity Framework
* MySQL

### System Requirements 
1. [.NET 5.0](https://dotnet.microsoft.com/download)  
1. [MySQL Community Server](https://dev.mysql.com/downloads/file/?id=484914)
1. [MySQL Workbench](https://dev.mysql.com/downloads/file/?id=484391)

### Installation
1. Clone the [HairSalon.Solution](https://github.com/Thisisjameswyn/HairSalon.Solution) Repository

    ### Set Up Required Database
    1. Launch MySQL Workbench and enter into root connection
    1. In the Administration tab, select `Data Import/Restore`
    1. Select `Import From Self-Contained File` and navigate to `/HairSalon.Solution/james_wyn.sql`
    1. For Default Target Schema select New and enter `cassandra_copp`
    1. Click `Start Import`

2. Add an `appsettings.json` file to the `HairSalon.Solution/HairSalon` directory and add the following:
```json
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=james_wyn;uid=root;pwd=YourPassword;"
  }
}
```
3. Replace YourPassword with your own MySQL password
4. To run the app in terminal, navigate to `HairSalon.Solution/HairSalon` directory and enter the command:
```cs
$ dotnet run
```
6. If the server does not automatically open enter localhost:5000 in the address bar of your web browser

## Known bugs

This application has no known bugs.

## License

[MIT](https://opensource.org/licenses/MIT)

Copyright (c) James Wyn 2021.

## Contact Information

[github.com/thisisjameswyn](http://github.com/thisisjameswyn)