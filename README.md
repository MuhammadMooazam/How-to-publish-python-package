# Publish Your Python Package on PyPI.org

Are you ready to share your Python package with the world? Follow these steps to publish it on PyPI.org.

# Publish Your Python Package on PyPI.org

Are you ready to share your Python package with the world? Follow these steps to publish it on PyPI.org.

1. **Create a Folder**: Make a folder on your Desktop (e.g., `package`).

2. **Package Folder**: Within the `package` folder, create a new folder with the name of your package (e.g., `saylani-ds`).

3. **Create Files**: Inside the `saylani-ds` folder, create the following files:
   - `license.txt`
   - `readme.txt`
   - `setup.py`

4. **Init File**: Create a file named `__init__.py` within the `saylani-ds` folder. This file will contain your entire library code.

5. **Setup.py Configuration**: In the `setup.py` file, write the following code.

    ```python
    from setuptools import setup
    
    setup (name="saylani-ds",
    version="0.1",
    description="this is a package",
    long_description="this is a very very long description",
    author = "Sir Qasim and Syed Muhammad Mooazam",
    packages = ["saylani-ds"],
    install_packages = []
    )
    ```

6. **Install Dependencies**: In the package folder, open your command prompt and execute the following commands.
    This will install the wheel package.
        ```bash
        pip install wheel
        ```

    This command creates binary distribution packages.
        ```bash
        python setup.py bdist_wheel
        ```

    This command builds the source distribution package and the binary distribution package.
        ```bash
        python setup.py sdist bdist_wheel
        ```

7. **Folder Creation**: After completing the previous steps, two folders will be automatically generated in the package folder.

8. **Update After Changes**: After making any changes to your Python files, ensure you update your packages. Run the following command each time.
    ```bash
    python setup.py sdist bdist_wheel
    ```

9. **Create a PyPI Account**: If you don't already have one, go to [https://pypi.org/](https://pypi.org/) and set up your PyPI account.

10. **Publish Your Package**: To publish your package on PyPI, follow these steps.
    - Install the `twine` package.
            ```bash
            pip install twine
            ```
    - Upload your package to PyPI using `twine`.
            ```bash
            twine upload dist/*
            ```

     When prompted, enter your PyPI account username and password.

11. **Package Successfully Uploaded**: Congratulations! Your package has been successfully uploaded to PyPI.

Now, your Python library is ready to be shared with the world. Enjoy the process!
