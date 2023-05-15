# VIRTUAL ENVIRONMENT IN PYTHON

1. **what is virtual environment (vev)?**
   - venv is python environment.
   - python interpreter, libraries, scripts installed into it.
   - It's **isolated** from other virtual environments.
   - by default, any python libraries installed in system, in **OS**.
   - **Example:**
      -  Down the line the if the libraries get updated so there may be a possibility that your code may fail or stop working.

1. **why do we need venv?**
   - To manage python packages for different projects

1. **Install Virtual environment**
   ```bash
   pip3 install virtualenv
   ```

1. **How to create venv?**

   ```bash
   python3 -m venv sample-project
   # or
   virtualenv sample-project


   # python3 --> To run python script
   # -m --> To run module
   # venv --> Name of the module
   ```

   - here **_sample-project_** refers to virtual environments name to be created
   - Once ran the above command new folder will be created
   - Now check python version using below command, which will show system python version
   ```bash
   python3 -V
   ```
1. **How to activate venv?**
   ```bash
   # To activate
   source sample-project/bin/activate

   # Then check python location
   which python

   # use below command to check the libraries of sample-environment (venv)
   pip3 list
   ```

1. **How to deactivate venv?**
   ```bash
   deactivate
   ```