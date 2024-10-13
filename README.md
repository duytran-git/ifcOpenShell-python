# IfcOpenShell-Exercise
## An exercise of IfcOpenShell

### The task:
From an IFC file (BIM4EEB-TUD-2x3.ifc), make a dictionary of all walls (IfcWallStandardCase) that have windows (IfcWindow), each wall described with its
- GUID
- dimensions
- the total window area of the wall

### The result of the assignment includes two file:
- A report of the assignment, explain what results you achieved and how you did it. The format of the report should be a .pdf file;
- The Python code with the format of .py file.

### Requirements of the Python code:
#### The main part of the code should be wrapped in the main() function, for example:
def main(model_path):

…

return walls_with_windows

The input should be the path to your IFC file, and the output should be a list including all walls with windows with the required info. Walls without windows cannot be in the list.

#### The format of the output should be like:
[{'Dimensions': #dimensions from propertyset of the wall,

'GlobalId': #GUID of the wall,

'WindowsArea': #the total window area of the wall },

{'Dimensions': {'Height': #height, 'Length': #length , 'Width': #witdth }

#dimensions from propertyset of the wall,

'GlobalId': #GUID of the wall,

'WindowsArea': #the total window area of the wall },

…]
