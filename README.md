# IMEJI SASS
## DESCRIPTION
imeji sass is the migration from classic css to the sass framework compass. It creates possibilities for smarter cross-instance modifications, because every instance needs for them application css only one file with variables and could include all other declarations from imeji default. You should only migrate the _vars.scss to your wished instance and have no trouble with changed or new core css declarations.


## STRUCTURE
the application.scss (app.scss) includes the variables (_vars.scss) and the "_combinedStyles.scss".

The _combinedStyles.scss includes all separated scss-files without the _vars.scss. That gives the advantage for other instance to include only the own variable.scss and the _combinedStyles.scss from imeji default without any knowledge of every file-hierachy separation.


## REQUIREMENTS
```
$ sass -v
Sass 3.3.8 (Maptastic Maple)
$ compass -v
Compass 0.12.6 (Alnilam)
Copyright (c) 2008-2014 Chris Eppstein
Released under the MIT License.
Compass is charityware.
Please make a tax deductable donation for a worthy cause: http://umdf.org/compass
```


## NOTICE
EVERY folder in root directory symbolize an instance of imeji and is a COMPASS project.


## COMPILE
for development it's recommended to use the compass watch job 
```
compass watch "path-to-your-working-directory/imeji_sass/compass-project/"
```
for other compilation as production or sth. else read the 'command line docu' http://compass-style.org/help/tutorials/command-line/ or http://compass-style.org/help/tutorials/production-css/


## INSTALL
You find a very practicable installation guide on http://www.compass-style.org/install/ .
If you get a failure (e.g. on Debian systems) with "$ gem update --system", please try the following steps in front of update system:
```
sudo gem install rubygems-update  
sudo update_rubygems
```
