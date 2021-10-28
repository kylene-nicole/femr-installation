# fEMR - Fast Electronic Medical Records

### Attention Developers - Need to update the instructions?
You can use the [editor on GitHub](https://github.com/kylene-phillips/femr-installation/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

## Description
fEMR is a fast EMR solution for remote clinics who depend on speed and ease of use rather than complex features. Check out [Team fEMR's website](https://teamfemr.org/) for more information and a live demo.

### Join our development community
1. Slack (will be updated soon!)
2. [JIRA](https://teamfemr.atlassian.net/jira/projects)
3. [Team fEMR](https://teamfemr.org/)

### Running the application using Docker
1. Make sure you have Docker installed and running on your machine.
2. Clone the femr repo and checkout the super-femr branch.
3. Cd into the super-femr directory: `cd super-femr/`.
4. Run `docker-compose up` to start the app.
5. If step 4 successfully finishes, the app will be available at http://localhost:9000/

## Installation Instructions

### Prepare Your System: Install Software and Dependencies
- [IntelliJ IDEA Ultimate](https://www.jetbrains.com/idea/download/#section=mac)
- [MySQL Server](https://dev.mysql.com/downloads/mysql/)
- [MySQL Workbench](https://dev.mysql.com/downloads/workbench/)

(hi Bat! I am roughly listing the order of operations I took so you can put the links + make it pretty :))
Play Framework
Scala
Restart InteliJ IDEA

Clone the repo, make a project
configure the perferences with play and scala
1.8 jdk language level to 8

Edit the conf

...
### Edit application.dev.conf 
```
include "application.conf"
settings.researchOnly=0
db.default.url="jdbc:mysql://127.0.0.1:3306/femr_db?characterEncoding=UTF-8"
db.default.username="testing"
db.default.password="password"
photos.defaultProfilePhoto="./public/img/defaultProfile.png"
csv.path="./Upload/CSV"
```

Setup the MySQL Server
Setup the MySQL Workbench
.....
### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/kylene-phillips/femr-installation/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
