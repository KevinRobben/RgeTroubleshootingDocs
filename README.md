# Read the Docs Template

This project serves as a quick-start project framework for rapidly deploying the ReadTheDocs project documentation software using the MkDocs engine. In this instance, the MkDocs project 'project' has already been deployed for you. You can continue with your deployment by editing the `*.md` files within the `/project` directory.


## Table of Contents
- [Background](#background)
- [Usage](#usage)


## [Background](#table-of-contents)

ReadTheDocs is an open-source ...

The MkDocs engine is an open-source ...


## [Usage](#table-of-contents)

To use the existing `/project` folder, skip step 5 and proceed to step 6.

1. Clone this repository and nagivate into it.

2. Delete the .git directory and initialize a new git project for your docs.
```BASH
rm -rf .git
git init
```

3. Create and activate a new Anaconda environment for your project.
```BASH
conda create -n docs-project --python=3.8
conda activate docs-project
```

4. Install the prerequisite software and check the MkDocs version.
```BASH
pip3 install -r requirements.txt
mkdocs --version
```

5. (optional) Delete the existing `/project` folder and initialize a new MkDocs project.
```BASH
rm -rf project
mkdocs new project
```

6. Within the `/project` folder is a configuration file called `/project/mkdocs.yml` as well as a folder `/project/docs` containing the documentation pages. Edit `mkdocs.yml` to change the look and layout of your documentation platform. Edit the files under the `docs` directory with the documentation content.

7. Run the local server to view your docs when you are ready.
```BASH
mkdocs serve
```

8. Connect to [localhost:8000](http://127.0.0.1:8000/) to preview your docs.

9. You can continue to edit the docs and MkDocs will automatically rebuild the site. Refresh the page to see your changes.

10. When you are ready to deploy the docs, build the static pages using MkDocs. This command will create a folder called `/project/site` with the HTML and CSS files to host the docs.
```BASH
mkdocs build
```



*Written by Austin Dial. Maintained by Seaborn.*
