# Project HALO: Database Design and Implementation


Project HALO is a database design and implementation project that provides basic structure and functionalities of real life database systems. The storing assets of the database form a hi- erarchy. Each record is stored inside pages, those pages are stored in files, and files are organized according to their types. The program builds those aspects in nonvolatile storage with system folders and files, so as records and types get updates the data can be reached after the termination. To simplify the project, all the search operations are made with respect to the primary key of data types. The pages inside folders are stored in a stored manner according to their pri- mary keys, which decreases search times significantly. This project offers a great variety of database functionalities from creating records to listing all records of any given type. The program reads user input line by line, processes through the database operations, and writes the requested result to a log file.


### Running the Program
- Clone the repository to your local or download the zip
- Open a terminal tab in the folder the code folder is in
- Install the requirements if necessary
- Run the following command: `python3 2017400210_2017400219_2018400045/src/haloSoftware.py <input_file.txt> <output_file.txt>`
- You will find the outputs in the provided output file.
- You will find the logs in the haloLog.csv file under the directory you run the command.

<i>Developed for CMPE321 Introduction to Database Systems course, Bogazici University, Spring 2021, together with Adalet Veyis Turgut and Ufuk Arslan<i>

