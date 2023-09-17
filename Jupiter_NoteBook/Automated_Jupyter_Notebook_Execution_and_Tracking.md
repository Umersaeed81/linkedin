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

# Automated Jupyter Notebook Execution and Tracking

The purpose of this Python code is to;
- Automate the execution of Jupyter notebooks.
- Track and identify any errors that occur during the execution process. 

The code achieves this by defining a function run_script(script_path) that executes Jupyter notebooks and then iterates through a list of script paths, executing each one and capturing any scripts that encounter errors. The identified error scripts are then printed at the end of the execution.

## Import required library


```python
import os
```

## User define function


```python
def run_script(script_path):
    return os.system(f'jupyter nbconvert --execute --to notebook --inplace {script_path}')
```

## List of script paths


```python
script_paths = [
    "C:/Users/uWX161178/Daily/SLA_Conformance/00_2G_Daily_Conformance.ipynb",
    "C:/Users/uWX161178/Daily/SLA_Conformance/03_2G_Week_Conformance_BH.ipynb",
    "C:/Users/uWX161178/Daily/SLA_Conformance/02_2G_Month_Conformance_BH.ipynb",
    "C:/Users/uWX161178/Daily/SLA_Conformance/01_2G_Quarterly_Conformance.ipynb",
    "C:/Users/uWX161178/Daily/SLA_Conformance/04_Cluster_DA_Month_Week_Level_KPIs.ipynb"
]
```

## Execute scripts and track errors


```python
error_scripts = []
for path in script_paths:
    return_code = run_script(path)
    if return_code != 0:
        error_scripts.append(path)
if error_scripts:
    print(f"The following scripts had errors: {error_scripts}")
```


```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/Jupiter_NoteBook/fig/Automated_Jupyter_Notebook_Execution%20_0.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/Jupiter_NoteBook/fig/Automated_Jupyter_Notebook_Execution%20_0.png?raw=true"/>




```python
Image(url='https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true')
```




<img src="https://github.com/Umersaeed81/linkedin/blob/main/log/sf_log.png?raw=true"/>


