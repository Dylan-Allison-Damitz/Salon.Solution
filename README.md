# Eau Claire's Salon 

#### By Dylan Allison-Damitz

## Technologies Used :floppy_disk:
* _NuGet Package Manager_
* _C#_
* _.Net 5_
* _REPL_
* _MySQL_
* _MySQL Workbench_

## Description :page_with_curl:
_A website for Eau Claire's salon that allows the salon owner to track current stylists and their customers, as well as add new stylists and customers_

## Setup/Installation Requirements :triangular_ruler:

* _Clone github repo: https://github.com/Dylan-Allison-Damitz/Salon.Solution.git_
* _Navigate into the directory from your desktop: cd Salon.Solution_
* _Open in Vs code: code ._
* _Navigate to the HairSalon directory using the terminal: cd HairSalon_
* _To install dependencies, run: dotnet restore_

## Importing the database

* In MySQL Workbench navigator, select 'Administration' in the top left corner, and then select 'Data Import/Restore'
* In the Import Options screen, select 'Import from Self-Contained file'
* Select the dump file titled 'dylan_allison_damitz.sql'
* Navigate to the Import Progress screen, and select the 'Start Import' button to begin import of the database file

## Updating appsettings.json

* Once you've imported the database, create an appsettings.json file in the HairSalon folder
* Copy and paste the following code into the file:

```
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=dylan_allison_damitz;uid={YOUR-USERNAME};pwd={YOUR-PASSWORD};"
  }
}
```
* Make sure you remove the curly brackets after entering in your username and password
* Once your databse connection is complete, return to the terminal and run 'dotnet build' to compile the project

## License :clipboard:
MIT &copy; 2021 _Dylan Allison-Damitz_
## Contact Information :mailbox:

_Dylan Allison-Damitz:
dylandamitz@gmail.com_
