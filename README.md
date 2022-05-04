Convert Json to PlantUML

This project is focused on the conversion of json files to PlantUML.
You can download the project with command git-clone + http address of this repository from branch master into your local directory.
Than you can open the directory in your preferred editor.
Main function contains input and output arguments with paths of folders. You need to add these arguments into Debug Configurations.

For example in Eclipse: Debug Configurations -> Arguments -> Program arguments and insert  -i C:\Test\Json  -o C:\Test\UML
Than copy directories Json and UML from directory of the project jsonParser into directory C:\Test

Now the main function can check whether it has all needed arguments for converting json files and creating new file PlantUML.
In the main function, all files from the Json folder are loaded first, the json file structure is mapped using the Object Mapper and the names of individual classes are extracted. The relationships between the classes are then verified with function validateAssociations. 
Then the file for writing PlantUML will open, where the individual classes with their relations will be written.

You can look at already created file plantUML.txt with result in the directory jsonParser.
