


## Section 1: Basic operations 

| Code                       | Description                                                                                  |
| :------------------------- | :------------------------------------------------------------------------------------------- |
| `pixi init`                | Start a new pixi environment                                                                 |
| `pixi install`             | Install everything from an existing environment using the `pixi.lock` and `pixi.toml` files. |
| `pixi add python=3.12 pip` | Install Python 3.12 and the pip installer into the environment                               |
| `pixi run <command>`       | Use the environment's dependencies to run a command line command.                            |
| `pixi shell`               | "Activate" an environment so that you don't have to type `pixi run`                          |
| <Delete .pixi folder>      | Remove the environment and all dependencies from the machine                                 |


**Exercises**

1. Open a new project folder in VSCode, in a new window.
2. Initialize a new Pixi project (you shuld see a `.pixi` folder)
3. Install Python 3.8 and pip into the environment.
4. Run `python --version` using the pixi environment (you should see `Python 3.8` in the output.)
5. Delete the pixi environment, without losing the `pixi.toml` file.
6. Reinstall everything from the `pixi.toml` file.


.
---
## Section 2: Installing Dependencies

| Code                                   | Description                                                                                                                  |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------- |
| `pixi add <package>`                   | Install a package from [conda-forge](https://conda-forge.org/packages/)                                                      |
| `pixi add --pypi <package>`            | Install a package from [PyPI](https://pypi.org/)                                                                             |
| `pixi add --git <url>`                 | Install a package from a git repository                                                                                      |
| `pixi remove <package>`                | Uninstall a package                                                                                                          |
| `pixi run python -m ipykernel install` | (Special for Python notebooks) Set up a Jupyter kernel for using notebooks with this environment (needs ipykernel from PyPI) |


**Exercises**

1. Create a pixi project and install `Python 3.11` and `pip` into it from Conda Forge
2. Install `numpy` and `pandas` from PyPI
3. Set up the environment so it works with jupyter notebooks using the ipykernel package, and check that you can import the package into your notebook.
4. Remove the `pandas` package from the environment.  Restart the notebook and confirm that you get an error when you try to import pandas.


.
---
## Section 3: Working with Multiple Sub-Environments

| Code | Description |
| :--- | :---------- |
| `pixi add -f <group> <package>` | install the package into a "feature" group. |
| `pixi project environment add <name> -f <group>` | set up an environment to use a given feature group. |
| `pixi run -e <name> <command>` | Run the terminal command using a given Pixi environment
| `pixi shell -e <name>` | "Activate" a given Pixi environment, so you don't need to write `pixi run`. |

**Exercises**

1. Create a pixi project with `Python 3.12` and `pip` in it from Conda Forge.
2. Install `numpy` and `matplotlib` from PyPI into the `data` feature group.
3. Create an environment (let's also call it `data`) and link it to the `data` feature group.
4. Run `python -c "import numpy; print(numpy.version)"` with the `data ` environment.
5. Run `python -c "import numpy; print(numpy.version)"` with the default environment.  You should get an error, as numpy wasn't installed there.
6. Create a `web` environment and features, which contains the `flask` PyPI package.  Confirm it's installed there and not elsewhere!
