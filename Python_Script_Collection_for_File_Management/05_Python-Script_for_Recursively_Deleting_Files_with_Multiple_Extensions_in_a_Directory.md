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

# Python Script for Recursively Deleting Files with Multiple Extensions in a Directory

This script is designed to perform a deep search and deletion of files with multiple specified extensions within the designated directory and its subdirectories.


```python
# import library
import os
# set folder path
working_directory = 'D:/Advance_Data_Sets/TXN_DataSets/GSM_CGID_log_Analysis'
# deleting excel and text file from folder and sub folders
for root, dirs, files in os.walk(working_directory):
    for filename in files:
        if filename.endswith(('.xlsx', '.txt')):
            os.unlink(os.path.join(root, filename))
```

The objective of this code achieves this by performing the following steps:
1. Imports the os module, allowing interaction with the operating system.
2. Sets the working_directory variable to a specific file path.
3. Utilizes a recursive loop (using os.walk) to navigate through all subdirectories and files within working_directory.
4. For each file encountered, checks if its filename ends with either .xlsx or .txt, indicating it is an Excel or text file.
5. If a file with one of these extensions is found, it is deleted from its respective location.


```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/Python_Script_Collection_for_File_Management/05_Python-Script_for_Recursively_Deleting_Files_with_Multiple_Extensions_in_a_Directory.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/Python_Script_Collection_for_File_Management/05_Python-Script_for_Recursively_Deleting_Files_with_Multiple_Extensions_in_a_Directory.png?raw=true"/>




```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true"/>


