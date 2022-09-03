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

Assumptions:
• All fields are be alphanumeric. Also, type and field names are be alphanumeric.
• User always enters valid input.
• The hardware of HALO center and HALO instances are built according to the blueprints.

Please refer to the report for further details.

### Running the Program
- Clone the repository to your local or download the zip
- Open a terminal tab in the folder the code folder is in
- Install the requirements if necessary
- Run the following command: `python3 2017400210_2017400219_2018400045/src/haloSoftware.py <input_file.txt> <output_file.txt>`
- You will find the outputs in the provided output file.
- You will find the logs in the haloLog.csv file under the directory you run the command.

<i>Developed for CMPE321 Introduction to Database Systems course, Bogazici University, Spring 2021, together with Adalet Veyis Turgut and Ufuk Arslan<i>

