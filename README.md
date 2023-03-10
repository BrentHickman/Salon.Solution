# HairSalon
#### An MVC web application for Hair Salons to track Stylists and their Clients

#### By Brent Hickman

## Technologies Used

* C#
* Dotnet 6
* Entity Framework Core
* MySQL
* Html
* Css


## HairSalon is an MVC application for Eau Claire's Salon. Users can add Stylists to their Salon list and can add Clients for each Stylist to help keep track of their appointments. 

## Setup/Installation Requirements

* Open a terminal window and clone this repository by entering into the command line:
> git clone https://github.com/BrentHickman/Salon.Solution.git
* In the terminal, navigate to the console application with the command:
> cd Salon.Solution/HairSalon
* Once in the "HairSalon" directory, create a new file called appsettings.json
* Within appsettings.json, put in the following code, replacing the [YOURUSERNAME] and [YOURPASSWORD] values with your own username and password for MySQL.
>{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=brent_hickman;uid=[YOURUSERNAME];pwd=[YOURPASSWORD];"
  }
}
* Next,launch MySQLWorkbench, navigate to the 'Administration' tab on the left and click 'Data Import/Restore'.
* On the 'Import Options' panel, select 'Import from Self-Contained File' and navigate to "brent_hickman.sql" located in the HairSalon directory.
* Then, on the 'Default Target Schema' panel select 'new' and name the import 'brent_hickman' and click 'ok'.
* Click the 'Start Import' button in the bottom right of the window and confirm the import is successful.
* To launch the application in development mode, enter the following lines into the command line:
> dotnet restore
* then:
> dotnet watch run
* The application should the be available at:
> https://localhost:5001/

## Known Bugs

* If you are experiencing any bugs, please contact me at brenthickman@ymail.com

## License

* [MIT](https://opensource.org/licenses/MIT)
* Brent Hickman 3/10/23