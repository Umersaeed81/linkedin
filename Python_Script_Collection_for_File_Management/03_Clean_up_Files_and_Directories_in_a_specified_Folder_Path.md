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

# Clean up Files and Directories in a specified Folder Path

The purpose of this code is to;
- **Clear Files and Directories:** It aims to remove all files and directories within a specified folder path.
- **Prevent Errors:** It checks if the folder path exists before attempting any operations to prevent potential errors.
- **Recursive Removal:** If a directory is found, it removes it along with all its contents recursively.
- **Clean-Up for Analysis:** This code might be used as a preparatory step before conducting analysis on a dataset, ensuring a clean slate for new data.


```python
import os
import shutil

folder_path = "D:/Advance_Data_Sets/TXN_DataSets/GSM_CGID_log_Analysis"

# Ensure the folder path exists before proceeding
if os.path.exists(folder_path):
    # Iterate over the contents of the folder
    for item in os.listdir(folder_path):
        item_path = os.path.join(folder_path, item)
        
        # If it's a file, remove it
        if os.path.isfile(item_path):
            os.remove(item_path)
            
        # If it's a directory, remove it and its contents recursively
        elif os.path.isdir(item_path):
            shutil.rmtree(item_path)
else:
    print(f"The folder path '{folder_path}' does not exist.")
```


```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/Python_Script_Collection_for_File_Management/03_Clean_up_Files_and_Directories_in_a_specified_Folder_Path.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/Python_Script_Collection_for_File_Management/03_Clean_up_Files_and_Directories_in_a_specified_Folder_Path.png?raw=true"/>




```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true"/>




```python

```
