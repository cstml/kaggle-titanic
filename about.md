This is my proper first attempt at a kaggle competition, and what better way to
start than the legendary Titatinc dataset.

But first thing first 

# Setting up the working environment
I chose to work in a virtual environment on my own laptop, running Ubuntu, and
using python3. To set up *Venv* I simply installed it from the apt

``` sudo apt install python3-venv ```

and then generated the Virtual Environment, named py3env with the use of venv
as a module of pyhton3.

``` 
python3 -m py3env 
```

To start working inside the virtual environment I simply activated it by doing

```
 source py3env/bin/activate 
```

I usually would use VIM for any text editing, but for this project I wanted to
try out jupyter-notebooks. 

The first thing i stumbled upon in this process was the fact that the jupyter-notebook
would not use the dependancies installed within the Virtual environment. With a quick google
I found out that in order to do this you must use a different Kernel inside the 
jupyter notebooks. To do this i needed to install (inside the venv) ipykernel
and add it to the Jupyter-notebook

```
pip install  ipykernel
python -m ipykernel install --user --name=py3env
```

This will install your virtual environment in 

```
/home/cstml/.local/share/jupyter/kernels/py3env
```

Which is the location of the Jupyter Notebooks kernels

Tidy.

-----
A bit more on the abov. If you want to uninstall the kernel from Jupyter 

```
jupyter kernelspec uninstall myenv
```

And to see the Jupyter kernels installed

```
jupyter kernelspec list
```
-----



