# Physics 360: Modern Astrophysics

This repository contains all materials for the Physics 360 course at Stanford. 

This include all the materials that contribute to the [course website](https://kipac.github.io/360/)

All content is managed and published using [quarto](quarto.org). 



We hope the setup of this repository could serve as a template also for some of our students. 
We think it could serve as a fairly general approach to organize ones scientific work mixing research, publishing, coding, version control, automatic backups, etc.  
Consequently we would appreciate any suggestions to improve the repo, its organization and its suggested workflow. 

In vscode or from the terminal we publish the quarto source to github.io pages using. 
```bash
quarto publish gh-pages
```

# Workflow

We can edit the .qmd files directly or follow the recipe below which does all the editing in jupyter notebooks but uses .qmd for the repository. 
We took this from [Berkleys DS100 course worflow](https://github.com/DS-100/course-notes).

#### Editing a note:

Convert the .qmd file to an .ipynb: ```quarto convert path/to/note.qmd```

Make edits on the .ipynb file

Preview notebook: ```quarto preview path/to/note.ipynb```

Convert to .qmd for rendering: quarto convert note_name.ipynb (must cancel quarto preview first)

Delete the path/to/note.ipynb and path/to/note.html

#### Rendering a Note:

Update _quarto.yml with the new note to be added

Render HTML docs: ```quarto render``` (must cancel quarto preview first)

check that the search.json file was generated. If not, quarto preview and click into every note.