# Readme
Example edit
This is the github repo of the [OsKOR group website](https://oskor.netlify.app/).

## Initial setup

### Install or upgrade R and RStuido

1. Install R for your OS from here: [https://cloud.r-project.org](https://cloud.r-project.org)
  - If you already have R installed you can check if your version is current by running the following from R console:
  ```
  R.version.string
  ```
2. Install RStudio Desktop for your OS from here: [https://www.rstudio.com/products/rstudio/download/#download](https://www.rstudio.com/products/rstudio/download/#download)
3. Update your R packages from the R console:
```
update.packages(ask = FALSE, checkBuilt = TRUE)
```
4. Install the [blogdown package](https://bookdown.org/yihui/blogdown/) in R:
```
if (!requireNamespace("remotes")) install.packages("remotes")
remotes::install_github("rstudio/blogdown")
```

### Install and set up Git

- Make a github account [here](https://github.com/).
- Ask Mateus ([g.m.bernardo.harrington@keele.ac.uk](mailto:g.m.bernardo.harrington@keele.ac.uk)) to be added as a collaborator to the repo.
- Make sure Git is installed on your machine (guide [here](https://happygitwithr.com/install-git.html))
- Add your username and email to git:
From the shell:
```
git config --global user.name 'Jane Doe'
git config --global user.email 'jane@example.com'
git config --global --list
```

Or from R with the [usethis package](https://usethis.r-lib.org/):
```
## install if needed (do this exactly once):
## install.packages("usethis")

library(usethis)
use_git_config(user.name = "Jane Doe", user.email = "jane@example.org")
```

Note that your user name doesn't need to be the same as your GitHub user name, though it can be, but your email ***must be the one*** associated with your GitHub account.
More details can be found [here](https://happygitwithr.com/hello-git.html)

- Optional, but recommended, step: [install a git client](https://happygitwithr.com/git-client.html)

I would highly recommend following chapters 4-14 of the [Happy Git with R book](http://happygitwithr.com/) if you are completely new to R and Git.

### Cloning the homepage repo

- Open your terminal and navigate to a directory where you'd like to clone the repository.
- Run this command in your terminal:
```
git clone https://github.com/H-Mateus/spinal-studies-rjah-site.git
```

### Install Hugo

This site uses the [Hugo static website generator](https://gohugo.io/), so you will need to install it.

- On Linux Hugo is available in most major repositories so you can install from there.
- On Mac you'll likely want to use `homebrew`, instructions for which can be found [here](https://brew.sh/).
- On Windows you'll want to stop making bad life choices. If you refuse, there is a docker container or you could use [Chocolatey](https://chocolatey.org/), instructions [here](https://gohugo.io/getting-started/installing/).
