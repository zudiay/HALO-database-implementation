# Project HALO: Database Design and Implementation


Project HALO is a database design and implementation project that provides basic structure and functionalities of real life database systems. The storing assets of the database form a hi- erarchy. Each record is stored inside pages, those pages are stored in files, and files are organized according to their types. The program builds those aspects in nonvolatile storage with system folders and files, so as records and types get updates the data can be reached after the termination. To simplify the project, all the search operations are made with respect to the primary key of data types. The pages inside folders are stored in a stored manner according to their pri- mary keys, which decreases search times significantly. This project offers a great variety of database functionalities from creating records to listing all records of any given type. The program reads user input line by line, processes through the database operations, and writes the requested result to a log file.


The design has a system catalog for storing the metadata and data storage units (files, pages, and records) for storing the actual data. The system design supports the following operations:

<br><b>HALO Definition Language Operations</b>:
• Create a type 
• Delete a type 
• Inherit a type 
• List all types
<br><b>HALO Authentication Language Operations</b>:
• Login to HALO
• Logout from HALO • Register in HALO
<br><b>HALO Management Language Operations</b>:
• Create a record
• Delete a record
• Search for a record (by primary key)
• Update a record (by primary key)
• List all records of a type
• Filter records by one of the attributes of a type <br>

<b>Assumptions:</b><br>
• All fields are be alphanumeric. Also, type and field names are be alphanumeric.<br>
• User always enters valid input.<br>
• The hardware of HALO center and HALO instances are built according to the blueprints.<br>
• Field names, and values cannot be longer than 20 characters. The maximum number of fields cannot be greater than 12.<br>

<b>Constraints:</b>
<br>• The data must be organized in pages and pages must contain records. The page and record structure is explained in the report.
<br>• Storing all pages in the same file is not allowed. When a file becomes free due to deletions, that file must be deleted.
<br>• Although a file contains multiple pages, it must read page by page when it is needed. Loading the whole file to RAM is not allowed.
<br>• The first attribute of all types in HALO software must be a string type, named as “planet” and its value for all records must be “E226 − S187”.
<br>• The primary key of a record should be assumed to be the value of the second field of that record.
<br>• Records in the files should be stored in descending order according to their primary keys.
<br>• There can only be one user logged in to HALO software at any time. Also, any definition and management operation can only be performed while being logged in. Therefore, any operation without a login to HALO should be logged with a username null.
<br>• Filter operation has a condition part, which can only filter the integer attributes and only less than <, greater than >, and equal = operators can be used to create a condition.
<br>• Search, update and deletion of records shall always be done by primary key.
<br>• When a type is deleted, all records of that type must be deleted.
<br>• Types must be listed by ascending type names. Note that the built-in sort functions do sorting case- sensitively by default. This means that the elements starting with uppercase letters come first in the order.


HALO software logs all authentication, definition, and management operations into a CSV file (namely haloLog.csv) which consists of 4 columns, namely username, occurrence, operation, and status. Username is the name of the current user, the occurrence is the string form of UNIX time, the operation is the string form of the whole operation line prompted in the console, status is the result of the operation. Log file must be persistent and never deleted when the HALO software is either stopped or restarted.


<i>Please refer to the report for further details.<i>

### Running the Program
- Clone the repository to your local or download the zip
- Open a terminal tab in the folder the code folder is in
- Install the requirements if necessary
- Run the following command: `python3 2017400210_2017400219_2018400045/src/haloSoftware.py <input_file.txt> <output_file.txt>`
- You will find the outputs in the provided output file.
- You will find the logs in the haloLog.csv file under the directory you run the command.

<i>Developed for CMPE321 Introduction to Database Systems course, Bogazici University, Spring 2021, together with Adalet Veyis Turgut and Ufuk Arslan<i>

