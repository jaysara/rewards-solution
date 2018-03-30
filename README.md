# rewards-solution
Zip file containing rewards-solution.

#### Zip file contents:
*	The zip file contains the source code and executable jar and this ‘ReadMe.doc’
*	The actual source code is under ‘Rewards’ folder.
*	Dressing-1.0-SNAPSHOT-jar-with-dependencies.jar

### How to Build :
•	To build from the source code. Unzip the file an navigate to the ‘Rewards’ folder.
o	Run ‘mvn –U clean install’ to build the project.
o	The jar file should have been created under ‘target’ folder.
### How to Run
•	You can choose to run the program by either using the new .jar file built from the last file or by using the one that is attached with this solution.

Following commands can be run.
```script
java -jar Dressing-1.0-SNAPSHOT-jar-with-dependencies.jar HOT 8, 6, 4, 2, 1, 7
```
•	Output: Removing PJs, shorts, shirt, sunglasses, sandals, leaving house
```script
java –jar Dressing-1.0-SNAPSHOT-jar-with-dependencies.jar COLD 8, 6, 3, 4, 2, 5, 1, 7
```
•	Output: Removing PJs, pants, socks, shirt, hat, jacket, boots, leaving house 
```script
java -jar target/Dressing-1.0-SNAPSHOT-jar-with-dependencies.jar HOT 8, 6, 6
```
•	Output: Removing PJs, shorts, fail 
```script
java -jar target/Dressing-1.0-SNAPSHOT-jar-with-dependencies.jar HOT 8, 6, 3
```
•	Output: Removing PJs, shorts, fail 
```script
java -jar target/Dressing-1.0-SNAPSHOT-jar-with-dependencies.jar COLD 8, 6, 3, 4, 2, 5, 7
```
•	Output: Removing PJs, pants, socks, shirt, hat, jacket, fail 
```script
java -jar target/Dressing-1.0-SNAPSHOT-jar-with-dependencies.jar COLD 6
```
Output: fail 

* The more information can be found in Readme.docx file with in zip file.
The project uses third party library (juul) that provided extended reduced operation (foldLeft is used in this project) that is not available in Java 8.
