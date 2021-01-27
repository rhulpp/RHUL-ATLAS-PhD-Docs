# RHUL-ATLAS-PhD-Docs
A repository to hold documentation of software tutorials for new PhD students in the RHUL ATLAS group.

## Dependencies

This project is built with the Python package `mkdocs`, which can be installed using the following command:

```
pip install mkdocs
```

## Adding Tutorials

To add tutorials to the repository, start by forking the repository. 

You can then add a markdown file containing your tutorial to the `docs/` directory. 

To make it accessible from the navigation menu, you need to add a line in `mkdocs.yml`, as follows:

```
nav:
	...
	...
	- <Tutorial name>: <Tutorial markdown file>
```

With these two steps complete, submit a pull request to get your changes approved and integrated into the main repository.

If you want to test your changes locally, you can run `mkdocs serve` from the folder containing the `mkdocs.yml` file to deploy a version of the project site to http://127.0.0.1:8000/

## Markdown Syntax
One can use the already existing markdown files and corresponding pages as examples for new pages. However, here are a few markdown syntax examples:

Chapters and sections:
```
# Chapter
## Section
### Subsection
```

Hyperlink:
```
[TheClickableText](TheActualLink.com)
```

E-mail contact link:
```
<John.Doe.2021@live.rhul.ac.uk>
```

List of bullet points:
```
- Item 1
- Item 2
- Item 3
```
Math block:
```
$$
\beta_{i} = 2.5 \times x
$$
```

Inline math mode:
```
Some text with an equation \( \alpha = \frac{x}{y} \) in the middle.
```

When including an image one needs to push it to the directory `docs/img`. Then one can render an image with:
```
![imagetitle](./img/someimage.jpg)
```


## Github Pages Integration

The project site is hosted live using Github pages at https://rhulpp.github.io/RHUL-ATLAS-PhD-Docs

To update the live version, checkout the master branch of the main repo, and then run the command `mkdocs gh-deploy`