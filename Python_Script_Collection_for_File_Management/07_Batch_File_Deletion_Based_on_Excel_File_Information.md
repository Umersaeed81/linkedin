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

# Batch File Deletion Based on Excel File Information

The purpose of this code is to;
- **Set Working Directory:** It sets the current working directory to a specified path.
- **Read Excel File:** It reads an Excel file named 'DA_Files.xlsx' that contains information about the files to be deleted.
- **Iterate Through Excel Rows:** It iterates through the rows of the DataFrame obtained from the Excel file.
- **Delete Files:** For each row, it checks if the specified file exists. If it does, it deletes the file and provides a success message. If it doesn't exist, it prints a message indicating this.
- **Completion Message:** After processing all rows, it provides a summary of the deletion process.
- **DA_Files.xlsx:** Format of the mentioned File is given below;


```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/Python_Script_Collection_for_File_Management/07_Batch_File_Deletion_Based_on_Excel_File_Information_Input_File_Format.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/Python_Script_Collection_for_File_Management/07_Batch_File_Deletion_Based_on_Excel_File_Information_Input_File_Format.png?raw=true"/>




```python
import os
import shutil
import pandas as pd

#set the Path 
path = 'D:/Advance_Data_Sets/File_Paths'
os.chdir(path)

# Read the Excel file
df = pd.read_excel('DA_Files.xlsx')

# Iterate through the rows and delete the files
for index, row in df.iterrows():
    file_path = row['File']
    if os.path.exists(file_path):
        os.remove(file_path)
        print(f"{file_path} deleted successfully")
    else:
        print(f"{file_path} does not exist")
```


```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true"/>


