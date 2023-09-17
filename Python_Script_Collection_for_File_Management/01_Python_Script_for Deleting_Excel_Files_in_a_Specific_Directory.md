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

# Python Script for Deleting Excel Files in a Specific Directory

This code is designed to perform a targeted cleanup by removing all Excel files from the specified directory. It could be useful when you need to clear out Excel files that are no longer needed or as a preparatory step for a new set of operations.


```python
import os
working_directory = 'D:/Advance_Data_Sets/TXN_DataSets/GSM_CGID_log_Analysis'
os.chdir(working_directory)
for filename in os.listdir(working_directory):
    if filename.endswith('.xlsx'):
        os.unlink(os.path.join(working_directory, filename))
```

This Python script that performs the following taks:
1. It imports the os module for interacting with the operating system.
2. The working_directory variable is set to a designated file path.
3. The current working directory is switched to the path specified in working_directory.
4. The script iterates through the files located in the working directory.
5. For each file, it verifies if it is a regular file (and not a directory).
6. If the item is indeed a file, it is subsequently removed from the directory.


```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/Python_Script_Collection_for_File_Management/01_Python_Script_for_Deleting_Excel_Files_in_a_Specific_Directory.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/Python_Script_Collection_for_File_Management/01_Python_Script_for_Deleting_Excel_Files_in_a_Specific_Directory.png?raw=true"/>




```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true"/>


