# Publish Your Python Package on PyPI.org

Are you ready to share your Python package with the world? Follow these steps to publish it on PyPI.org and let your code shine!

## Getting Started

1. **Create a Folder**: Start by creating a folder on your Desktop (e.g., `package`).

2. **Package Folder**: Within the `package` folder, give life to your project by creating a new folder with the name of your package (e.g., `saylani-ds`).

3. **Create Essential Files**: Inside the `saylani-ds` folder, craft the following essential files:
   - `license.txt`
   - `readme.txt`
   - `setup.py`

4. **The Heart of Your Package**: Create a file named `__init__.py` within the `saylani-ds` folder. This file is where the magic happens - write your entire library code here.

## Configuration and Dependencies

5. **Setup.py Configuration**: Open `setup.py` and pour in your package's vital information. Here's an example:
   
    ```python
    from setuptools import setup
    
    setup (name="saylani-ds",
    version="0.1",
    description="This is a package",
    long_description="A very, very long description of your amazing package.",
    author = "Sir Qasim and Syed Muhammad Mooazam",
    packages = ["saylani-ds"],
    install_packages = []
    )
    ```

6. **Install Dependencies**: In the package folder, fire up your command prompt and execute these commands to set the stage for your package:
   
   - Install the "wheel" package:
   
        ```bash
        pip install wheel
        ```

   - Create binary distribution packages:

        ```bash
        python setup.py bdist_wheel
        ```

   - Build the source distribution package and binary distribution package:

        ```bash
        python setup.py sdist bdist_wheel
        ```

## Package Progress

7. **Folder Wonderland**: After the previous steps, watch as two folders magically appear in the package folder.

8. **Stay Updated**: Whenever you make changes to your Python files, keep your packages updated by running this command:

    ```bash
    python setup.py sdist bdist_wheel
    ```

## Share the Magic

9. **Create a PyPI Account**: If you don't already have one, embark on your journey at [PyPI.org](https://pypi.org/) and set up your PyPI account.

10. **Publish Your Package**: It's showtime! Share your package with the world by following these steps:

    - Install the "twine" package:
   
        ```bash
        pip install twine
        ```
   
    - Upload your package to PyPI using "twine":
   
        ```bash
        twine upload dist/*
        ```

    When prompted, enter your PyPI account username and password.

## Success!

11. **Package Successfully Uploaded**: Bravo! Your package has been successfully uploaded to PyPI, and now it's ready to shine in the Python ecosystem.

Now, your Python library is primed and polished for its grand debut. Share your creation with fellow developers and let the coding adventures begin!
