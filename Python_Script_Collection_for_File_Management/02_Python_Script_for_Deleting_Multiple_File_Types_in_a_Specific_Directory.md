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

# Python Script for Deleting Multiple File Types in a Specific Directory

This script facilitates the targeted removal of specific file types from the designated directory.


```python
import os

working_directory = 'D:/Advance_Data_Sets/TXN_DataSets/GSM_CGID_log_Analysis'
os.chdir(working_directory)

for filename in os.listdir(working_directory):
    if filename.endswith(('.xlsx', '.txt')):
        os.unlink(os.path.join(working_directory, filename))
```

The objective of this Python code is to clear (delete) files with either the .xlsx or .txt extensions in a specific directory. The code achieves this by performing the following steps:
1. Imports the os module to interact with the operating system.
2. Sets the working_directory variable to a specified file path.
3. Changes the current working directory to the path specified in working_directory.
4. Iterates through the files in the working directory.
5. For each file, checks if its filename ends with either .xlsx or .txt, indicating it is an Excel or text file.
6. If the file has one of these extensions, it is deleted.


```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/Python_Script_Collection_for_File_Management/02_Python_Script_for_Deleting_Multiple_File_Types_in_a_Specific_Directory.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/Python_Script_Collection_for_File_Management/02_Python_Script_for_Deleting_Multiple_File_Types_in_a_Specific_Directory.png?raw=true"/>




```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true"/>


