# pyNIO-test

This is a repository to host a recipe to built a conda environment with pyNIO, Xarray and Matplotlib (among other) packages.

There are a few ways to create this environment:

1. By using the `spec-file.txt` file:

    ```
    $ conda create --name myenv --file spec-file.txt
    $ pip install matplotlib
    ```

    * **Note:** This command will create a new environment. Change `myenv` to a new environment name.

    or,

    ```
    $ conda install --name myenv --file spec-file.txt
    $ pip install matplotlib
    ```

    * **Note:** This command will install packages in an existing environment. Change `myenv` to an existing environment name.

    * **Reference:** [https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)

2. By using the `environment.yml` file:

    ```
    $ conda env create -f environment.yml
    ```

    * **Note:** This command will create a new environment with name `pyNIO`. To change it, edit the `environment.yml` file before running the command.

    * **Reference:** [https://shandou.medium.com/export-and-create-conda-environment-with-yml-5de619fe5a2](https://shandou.medium.com/export-and-create-conda-environment-with-yml-5de619fe5a2)


After setting up the environment, use the provided data and jupyter notebook to test the packages:

```
$ jupyter-lab Untitled.ipynb
```

And run the cells therein.

