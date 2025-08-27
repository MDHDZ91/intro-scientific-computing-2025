# Class Environment Setup (Week 0)

This short module gets everyone on the same Python setup so notebooks run the same for all students.
In general when working on projects it is smart to have dedicated env that help to contain all the packages you need.
This allows for a cleaner set-up that can be shared with others.


If you followed instruction on the github repo you have miniforge already so these commands should work. 


Open your terminal.

### 1) Create the class environment
```bash
mamba create -n py101 python=3.12 -c conda-forge -y
```

### 2) Activate it
```bash
mamba activate py101
```

### 3) Install course packages
```bash
mamba install -c conda-forge numpy pandas matplotlib seaborn jupyterlab ipykernel cartopy -y
```

### 4) Register the kernel for Jupyter
```bash
python -m ipykernel install --user --name py101 --display-name "Python (py101)"
```

### 5) Launch Jupyter - this contains both jupyter notebook and jupyter lab 
```bash
jupyter lab
```
E