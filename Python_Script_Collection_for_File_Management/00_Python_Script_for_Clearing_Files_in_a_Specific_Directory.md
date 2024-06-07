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

# Python Script for Clearing Files in a Specific Directory

The code is designed to clear out all the files in the specified directory (working_directory). This could be useful in situations where you want to clean up a directory before performing a new set of operations, or if you need to remove temporary or outdated files.


```python
# Import Library
import os
# Set working directory path
working_directory = 'D:/Advance_Data_Sets/TXN_DataSets/GSM_CGID_log_Analysis'
os.chdir(working_directory)
# Python Script for Clearing Files in a Specific path
for filename in os.listdir(working_directory):
    file_path = os.path.join(working_directory, filename)
    if os.path.isfile(file_path):
        os.remove(file_path)
```

This Python script that performs the following tasks:
1. Imports the os module.
2. Sets the working_directory variable to a specific file path.
3. Changes the current working directory to the path specified in working_directory.
4. Iterates through the files in the working directory.
5. For each file, it checks if it's a regular file (not a directory).
6. If it's a file, it removes it.





