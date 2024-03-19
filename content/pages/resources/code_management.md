---
weight: 3
---

# Code Management

For a project to span multiple semesters, it is important that the code and documentation for the project be accessible by the instructor and easy to hand off to the next team for future development. Git combined with a Git hosting website is the current industry standard for version control, and thus the logical solution for code management. Git repositories can easily be migrated from one site to another, so the choice of hosting service is not terribly important in the long term, but since GitHub is the most popular Git host and offers upgraded plans to educators for free, it is a fine choice. Other sites such as GitLab and Bitbucket would work as well, but this document assumes code will be managed under GitHub. 

## GitHub Organizations 

A GitHub organization consists of users and repositories. By creating an organization for a class and adding all of the students to the organization, all the class’s projects can be organized in one place, and the instructor does not need to keep track of repositories scattered among various student accounts. 

As an educator, it is possible to create an organization and then have it upgraded to the “GitHub Team” tier for free through https://education.github.com/. This provides more features than the free tier, such as protected branches, multiple reviewers in pull requests, and more CI/CD minutes per month. 

## Documentation 

Markdown files are well-suited for documentation for future developers such as instructions for environment configuration, installation of dependencies, and deployment. Markdown is a plain text format, so the files are well-managed by Git, and the documentation renders nicely when browsed on GitHub. 

Binary files such as images, Word documents, and PDF documents, are not as well suited for management under Git, and can result in a bloated repository size if changes to such files are frequently committed over time. However, having all documentation files in the same location can be advantageous for organization purposes, so if students need to produce documents in a binary format as part of the project, the instructor should decide how they want to handle those, and clearly communicate to the students how the documents should be delivered. 

## Other Considerations 

Some other things to consider when making decisions about code management are: 

* If the commit history of a project will be important, it is more important to ensure that students are using good Git practices. If not, the history can simply be deleted before handing the project off to the next team. 

* Requiring students to create a .gitignore before adding any files to a new repository can help keep the Git history clean from things like Python virtual environments and IDE configurations 

* Discuss code management with project partners before the project begins. Many partners will not care about this aspect, but others may have preferences (or even legal reasons) for specific policies about code management and delivery 

{{< footer >}}
 
