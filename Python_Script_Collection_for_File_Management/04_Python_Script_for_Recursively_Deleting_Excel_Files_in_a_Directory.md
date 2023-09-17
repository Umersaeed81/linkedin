```python
from IPython.display import Image
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/log/t_log.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/log/t_log.png?raw=true"/>



#  [Umer Saeed](https://www.linkedin.com/in/engumersaeed/)
Sr. RF Planning & Optimization Engineer<br>
BSc Telecommunications Engineering, School of Engineering<br>
MS Data Science, School of Business and Economics<br>
**University of Management & Technology**<br>
**Mobile:**     +923018412180<br>
**Email:**  umersaeed81@hotmail.com<br>
**Address:** Dream Gardens,Defence Road, Lahore<br>

# Python Script for Recursively Deleting Excel Files in a Directory

The objective of this Python code is to recursively traverse through a specified directory and delete all files with the .xlsx extension. 


```python
# import library
import os
# set path
working_directory = 'D:/Advance_Data_Sets/TXN_DataSets/GSM_CGID_log_Analysis'
# delete excel fild from folder and sub folders
for root, dirs, files in os.walk(working_directory):
    for filename in files:
        if filename.endswith('.xlsx'):
            os.unlink(os.path.join(root, filename))
```

The objective of this code achieves this by performing the following steps:
- Imports the os module, enabling interaction with the operating system.
- Sets the working_directory variable to a specific file path.
- Utilizes a recursive loop (using os.walk) to navigate through all subdirectories and files within working_directory.
- For each file encountered, checks if its filename ends with .xlsx, identifying it as an Excel file.
- If an Excel file is found, it is deleted from its respective location.


```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/Python_Script_Collection_for_File_Management/04_Python_Script_for_Recursively_Deleting_Excel_Files_in_a_Directory.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/Python_Script_Collection_for_File_Management/04_Python_Script_for_Recursively_Deleting_Excel_Files_in_a_Directory.png?raw=true"/>




```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true"/>


