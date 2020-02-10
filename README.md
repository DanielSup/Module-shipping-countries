# Simple module and webpage for showing information about countries and shipping methods

This repository contains source code of my simple module for Opencart version 1.5.6.4 for showing the list of countries and for each country possible shipping methods. You can see this module on the website [https://www.flakon.cz/index.php?route=countries/countries](https://www.flakon.cz/index.php?route=countries/countries).

In the file `ceny a doba dopravy.csv` in the directory `catalog/model/countries` there is information about countries and possible shipping methods for countries with fee and cash on delivery fee (if it is possible to pay by cash on delivery for the combination of shipping method and country). The model in the file `countries.php` works with this file. In the same directory there are php files with model classes representing a country and shipping method. The object of type `Country` contains the list of shipping methods.

The `catalog` directory also contains `controller` directory with the controller which works with the models mentioned above. The controller gives all the information to the template in the `catalog/view/default/theme/template/countries` directory and gets important strings from the `catalog/language` directory with php files for each language.