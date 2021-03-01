# Snaps used
•	File Reader – to access “Trng_FilterEven.csv”
•	CSV Parse – to parse  “leads.csv”
•	Copy – because I need 2 outputs (output 3.0 and 3.1) 

Task_3.0
•	Filter – only records that has even index “$['Employee ID'] % 2 == 0”
•	Mapper – for $Name, $EmployeeID && $DepartmentID
•	CSV Formatter – to format in CSV
•	File Writer – in “Trng_FilterEven.csv”

Task_3.1
•	Router – (Outrput0) to check $['Employee ID'] < 15
Router – (Outrput1) “ELSE” !($['Employee ID'] < 15) 

Output0 || ‘<15’
•	CSV Formatter – to format in CSV
•	File Writer – in “Trng_IDbelow15.csv”

Output1 || ‘Else’
•	CSV Formatter – to format in CSV
•	File Writer – in “Trng_IDabove15.csv”
