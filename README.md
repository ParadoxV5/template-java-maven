# `template-java-maven`

Built upon [`ParadoxV5/java-mystring`](https://github.com/ParadoxV5/java-mystring),
this is a basic yet thorough template for a Maven-managed Java project.


## How to Setup

* _Delete [`src/main/java/.gitkeep`](src/main/java/.gitkeep), the filler file for the otherwise-empty folder)_
* Update the [`pom.xml`](pom.xml) with your project’s information (See [§`pom.xml`](#pomxml))
* Overwrite this `README` with an introduction to your epic project
* Replace *this template’s* [`LICENSE.txt`](LICENSE.txt) with
  [one](https://choosealicense.com/) that engraves your honor for posterity


## What’s inside

###### [`src/**`](src/)
The included setup implements the Maven Standard:

| Folder                           | Purpose                                                     |
|----------------------------------|-------------------------------------------------------------|
| [`src/main/java`](src/main/java) | Java sources for your app or library                        |
| `src/main/resources`             | Resources your app or library utilizes (e.g., images)       |
| `src/test/java`                  | Java sources for testing your project (e.g., JUnit Testing) |
| `src/test/resources`             | Resources your project testing uses                         |

###### [`pom.xml`](pom.xml)
The `pom` is [the Maven project metadata file](https://maven.apache.org/pom.html).
I have prepared blanks for project information near the top for you to fill in.

The following is a list (ordered by their appearance in the file) of handy
configurations I have also bundled in the metadata.
There might be bells and whistles that your project doesn’t need,
and you are welcome to remove those auxiliaries from your project’s `pom.xml`.

1. Developer and license information
2. Linking of supplementary (e.g., dependencies’) JavaDocs
3. [Execution plugin for Maven](https://www.mojohaus.org/exec-maven-plugin/)
4. [JetBrains annotations](https://github.com/JetBrains/java-annotations) (for code analysis)
   and [JUnit 5](https://junit.org/junit5/) Jupiter dependencies
5. Version Control, Deployment and Issue Management URLs metadata

###### [`LICENSE.txt`](LICENSE.txt)
See [§License](#License)

###### [`README.md`](README.md)
You are reading this right now…

###### [`.github/workflows/*`](.github/workflows)
Inside this folder are thoroughly configured (no modification required)
[GitHub Actions](https://github.com/features/actions) scripts that enable basic continuous deployment:

* [`packages.yml`](.github/workflows/packages.yml) –
  [Publish to GitHub Packages](https://docs.github.com/en/actions/publishing-packages/publishing-java-packages-with-maven#publishing-packages-to-github-packages)
  after a GitHub Release is published.
* [`pages.yml`](.github/workflows/pages.yml) – Generate Javadocs and
  [publish to GitHub Pages](https://github.blog/changelog/2022-07-27-github-pages-custom-github-actions-workflows-beta/)
  after the `main` branch receives a code update in the Java sources folder [`src/main/java`](src/main/java).

###### [`.gitignore`](.gitignore)
[The `.gitignore` file](https://git-scm.com/docs/gitignore) lists file patterns to exclude from Git’s records.

* `target` is the build output folder in the Maven Standard.
  Java must compile sources to Bytecode before interpreting them.
* Don’t include IDE (e.g., [IntelliJ IDEA](https://www.jetbrains.com/idea/) or
  [Eclipse IDE](https://www.eclipse.org/ide/)) configurations
  unless you want to enforce your organization’s digital environment.


## License

I have determined that this template is all traditional knowledge and no copyrightable production.
Therefore, I am licensing this template under the infamous [WTFPL](http://www.wtfpl.net/).