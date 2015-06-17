# Maven-Repo

Repository for maven artefacts (artifactory) for unified views dependencies

Usage of maven repo on github is described in http://kwebble.com/blog/2014/02/19/use-github-to-host-your-own-maven-repo

## How to add repository into project

These lines have to be added into pom.xml of the project into ```<repositories>``` section:

```
    <repository>
        <id>UnifiedViews_Maven_Repo</id>
        <name>UnifiedViews Git based maven repo</name>
        <url>https://github.com/UnifiedViews/Maven-Repo/tree/master/</url>
    </repository>
```

## How to add new file into the repo

Recommended is to add new file in extra branch, then to create pull request with description of reason why is such file needed.
For non-contributors it is expected to create issue with request to add some file into repo with version and additonal necessary info.

To add jar file into repo, these are steps
* clone this repository
* checkout master
* create branch
* install jar file into the cloned repository
* add all newly added files and commit
* push back into github the branch
 
