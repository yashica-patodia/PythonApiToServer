# PythonApiToServer


The goal of this assignment is to automatically generate a python fastapi server routes from python functions defined in a class and deploy it over a serverless framework like Vercel / AWS Lambda. All functions with @api decorator will automatically become apis defined in fastapi code.


# Contents of Directory
### File Structure


+-- YashicaLibrary\
|&ensp;   +-- __init__.py\
|&ensp;   +-- FastAPI.py\
|&ensp;   +-- FileHandling.py\
|&ensp;   +-- LambdaService.py\
+-- build\

+-- CustomUserService.py\
+-- main.py\



### Contents of each file


- YashicaLibrary\
    This is python package which contains a base class LambdaService which the users will have to extend to generate the FastAPI code.The user needs to write a code snippet similar to the one given in CustomUserService.py.

YashicaLibrary build --file CustomUserService.py

On executing the above command, it will generate the corresponding fastapi code in a folder called build inside the directory in which CustomUserService.py file is present.


