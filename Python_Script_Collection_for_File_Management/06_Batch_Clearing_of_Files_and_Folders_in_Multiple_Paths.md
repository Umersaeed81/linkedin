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

# Batch Clearing of Files and Folders in Multiple Paths

The purpose of this code is to;
- **Iterate Through Multiple Folder Paths:** It contains a list of folder paths, and it iterates through each path to perform the file and folder deletion operation.
- **Ensure Path Existence:** Before attempting any operations, it checks if the specified folder path exists to avoid potential errors.
- **Recursively Delete Directories:** If a directory is encountered, it removes the directory along with all its contents in a recursive manner.
- **Provide Feedback for Nonexistent Paths:** If a specified folder path does not exist, it prints a message indicating this.


```python
import os
import shutil
def delete_all_files_and_folders(folder_path):
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
# List of folder paths
folder_paths = ["D:/Advance_Data_Sets/License/LTE_NodeB_Level",
                "D:/Advance_Data_Sets/RF_Export/GSM/00_Frequency_Export",
                "D:/Advance_Data_Sets/RF_Export/GSM/01_NBR_Export",
                "D:/Advance_Data_Sets/RF_Export/GSM/03_GTRX_Export",
                "D:/Advance_Data_Sets/RF_Export/GSM/04_Cell_Export",
                "D:/Advance_Data_Sets/RF_Export/LTE/Cell",
                "D:/Advance_Data_Sets/RF_Export/UMTS/00_Cell_Export",
                "D:/Advance_Data_Sets/RF_Export/UMTS/01_NBR_Export",
                "D:/Advance_Data_Sets/RF_Export/GSM/01_NBR_Export",
                "D:/Advance_Data_Sets/RF_Export/GSM/03_GTRX_Export",
                "D:/Advance_Data_Sets/RF_Export/GSM/04_Cell_Export",
                "D:/Advance_Data_Sets/Output_Folder"]  

# Delete all files and folders in each path
for path in folder_paths:
    delete_all_files_and_folders(path)
```


```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true"/>


