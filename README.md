# general-template
A general Python project template for MF-DAS

After initializing your project from this template I would advice to do the following:

* Enable GitHub Pages by going to `Settings` -> `Pages` and under `Build and deployment` subsection `Source` choose `GitHub Actions` instead of `Deploy from a branch`.
* Change the name of your package by checking out the project and doing `git mv src/project_name src/your_actual_project_name` where `your_actual_project_name` is the name you chose for your project. After that `git commit -am "change package name"` and `git push`.
* Change the project name and other information in the `pyproject.toml`.
* Open .githubt/workflows/pdoc.yml in an editor and change `project_name` to the proper project name.

The template will take care of building and publishing project documentation from Python docstrings. You need to use the the `numpy` docstring format. Find the description of it [here](https://numpydoc.readthedocs.io/en/latest/format.html). The documentation will be built and published under dlr-mf-das.github.io/general-template where you need to replace `general-template` with your repository name.
