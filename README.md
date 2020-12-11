# RHUL-ATLAS-PhD-Docs
A repository to hold documentation of software tutorials for new PhD students in the RHUL ATLAS group.

#Dependencies

This project is built with the Python package `mkdocs`, which can be installed using the following command:

```
pip install mkdocs
```

#Adding Tutorials

To add tutorials to the repository, start by forking the repository. 

You can then add a markdown file containing your tutorial to the `docs/` directory. 

To make it accessible from the navigation menu, you need to add a line in `mkdocs.yml`, as follows:

```
nav:
	...
	...
	- <Tutorial name>: <Tutorial markdown file>
```

With these two steps complete, submit a pull request to get your changes approved and integrated into the main repository

#Github Pages Integration

The project is hosted live using Github pages at <rhulpp.github.io/RHUL-ATLAS-PhD-Docs>