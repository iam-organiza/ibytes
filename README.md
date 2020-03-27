# ibytes code sample

all code logic starts from init.php file
/core/init.php from the root directory

from there
I turned on output buffering 
include database connection
autoload all my class files
instantiate all my classes
then i created a global variable $pdo which is passed to all my classes except for the geoPlugin class
set default timezone
then i defined a constant BASE_URL which holds a string containing the url to my root folder
then i ran a foreach loop including every file from a folder called handlers which handles all my POST and GET requests

with all this set i just need to include init.php from anywhere in my project files to use all my classess and handlers
every other folder outside the core folder are my public folders where assets for the project are found
