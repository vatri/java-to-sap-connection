# java-to-sap-connection
Connect Java application to SAP and fetch a table.

## Requirements:

  1. SAP JCO ZIP with JAR and DLL files (make sure you have downloaded correct architecture)
  2. DLL path is added to PATH system environment variable
  3. JDK and JRE 8
  
## How to run

  - Run "git pull [THIS REPO URL]" in your CMD/terminal
  - Open the folder in IDE
  - Add JAR to build path
  - Update connection parameters in SapConn.java source file 
  - Open your SAP R/3 system and create Z_JCO_TEST function module with params: import-PI_PARAM (char); TABLE-PO_OUT (structure with fields MANDT, NAME and BIRTH)
  - Compile and run using IDE tools
  - Open http://localhost:8080/
  - Enter your SAP password and hit enter
  - Now you should get JSON with list of all employees from HR module
