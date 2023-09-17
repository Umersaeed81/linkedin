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

Exercise caution when running this script, as it permanently deletes the subfolders and their contents in the specified directory. Always have a backup or work with test data when performing file operations.

## 1. Clearing Subfolders in a Specific Path

The objective of this Python script is to clear all subfolders within the specified working_directory. It iterates through the items in the directory and, for each subfolder, checks if it's a directory. If so, it recursively removes it along with all its contents.


```python
# import libraries
import os
import shutil

# set path
working_directory = 'D:/Advance_Data_Sets/TXN_DataSets/GSM_CGID_log_Analysis'
os.chdir(working_directory)

# Python Script for Clearing Subfolders in a Specific path
for subfolder in os.listdir(working_directory):
    subfolder_path = os.path.join(working_directory, subfolder)
    if os.path.isdir(subfolder_path):
        shutil.rmtree(subfolder_path)
```

## 2. Python Script for Clearing Empty Subfolders in a Specific path

The purpose of this Python script is to identify and remove any empty subfolders within the specified working_directory. It navigates through the items in the directory, and for each subfolder, it checks if it's a directory and if it's empty. If both conditions are met, the subfolder is recursively removed.


```python
# import libraries
import os
import shutil

# set path
working_directory = 'D:/Advance_Data_Sets/TXN_DataSets/GSM_CGID_log_Analysis'
os.chdir(working_directory)

# Python Script for Clearing Empty Subfolders in a Specific path
for subfolder in os.listdir(working_directory):
    subfolder_path = os.path.join(working_directory, subfolder)
    if os.path.isdir(subfolder_path):
        if not os.listdir(subfolder_path):  # Check if subfolder is empty
            shutil.rmtree(subfolder_path)
```

## 3. Recursive Empty Subfolder Remover

The purpose of this Python script is to identify and remove any empty subfolders within the specified working_directory. It defines a function that uses os.walk to navigate through the directory tree, and for each directory, it checks if it's empty. If so, the empty subfolder is removed.


```python
# import libraries
import os
import shutil


def remove_empty_subfolders(folder):
    for root, dirs, files in os.walk(folder, topdown=False):
        for dir in dirs:
            subfolder_path = os.path.join(root, dir)
            if not os.listdir(subfolder_path):
                shutil.rmtree(subfolder_path)

# set path               
working_directory = 'D:/Advance_Data_Sets/TXN_DataSets/GSM_CGID_log_Analysis'
remove_empty_subfolders(working_directory)
```

## 4. Delete excel files from subfolders

The objective of this Python script is to go through the subfolders within the specified working_directory. For each file in these subfolders, it checks if it has the .xlsx extension. If so, and the file is not in the root directory, it is deleted.


```python
# import libraries
import os
# set path
working_directory = 'D:/Advance_Data_Sets/TXN_DataSets/GSM_CGID_log_Analysis'

# Delete excel files from subfolders
for root, dirs, files in os.walk(working_directory):
    for filename in files:
        if root != working_directory and filename.endswith('.xlsx'):
            os.unlink(os.path.join(root, filename))
```

## 5. Delete excel and text files from subfolders

The objective of this Python script is to go through the subfolders within the specified working_directory. For each file in these subfolders, it checks if it has either the .xlsx or .txt extension. If so, and the file is not in the root directory, it is deleted.


```python
# import libraries
import os

# set path
working_directory = 'D:/Advance_Data_Sets/TXN_DataSets/GSM_CGID_log_Analysis'

# Delete excel and text files from subfolders
for root, dirs, files in os.walk(working_directory):
    for filename in files:
        if root != working_directory and filename.endswith(('.xlsx','.txt')):
            os.unlink(os.path.join(root, filename))
```


```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true"/>


