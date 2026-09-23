# CSSE332 — Operating Systems

Operating systems course materials, exercises, homework, labs, and supporting website files for CSSE332 at Rose-Hulman Institute of Technology.

This repository is a fork of [RHIT-CSSE/csse332](https://github.com/RHIT-CSSE/csse332). It combines course-provided material, starter code, examples, and solutions. Individual files and Git history should be consulted when distinguishing original coursework from supplied material.

## Start here

- Read the [syllabus](syllabus.md) for the course structure.
- Use [homeworks/](homeworks/) and [labs/](labs/) to find individual assignments.
- Refer to [ClassMaterials/](ClassMaterials/) and [notes/](notes/) for background explanations and examples.
- Use [docs/](docs/) and [labs/wsl/](labs/wsl/) for environment and course setup information.

## Repository guide

| Path | Contents |
| --- | --- |
| [ClassMaterials/](ClassMaterials/) | Lecture slides, activities, and example programs |
| [activities/](activities/) | Classroom activities |
| [homeworks/](homeworks/) | Assignment instructions, starter code, and exercises |
| [labs/](labs/) | Numbered labs and environment setup |
| [notes/](notes/) | Additional course notes |
| [sample_exams/](sample_exams/) | Practice exams and supplied solutions |
| [autograder/](autograder/) | Course grading support and associated source |
| [docs/](docs/) | Supporting course documentation |
| [Admin/](Admin/) | Course schedule-generation and administrative files |
| `_layouts/`, `_includes/`, `_data/`, `assets/` | Jekyll website templates, data, and assets |

## Topics represented

The collection includes C pointers and Makefiles, process creation and IPC, user/kernel threads, synchronization, mutexes, semaphores, condition variables, CPU scheduling, deadlocks, filesystems, paging, virtual memory, and memory-management exercises.

Examples of assignment entry points:

| Directory | Subject |
| --- | --- |
| [00_pointer_practice](homeworks/00_pointer_practice/) | C pointer practice |
| [03_simple_shell](homeworks/03_simple_shell/) | Shell implementation |
| [04_process_lab](homeworks/04_process_lab/) | Process exercises |
| [06_ext2](homeworks/06_ext2/) | Filesystem work |
| [07_mutex_basics](homeworks/07_mutex_basics/) | Mutexes |
| [08_semaphores_homework1](homeworks/08_semaphores_homework1/) and [09_semaphores_homework2](homeworks/09_semaphores_homework2/) | Semaphores |
| [10_hybrid_threads](homeworks/10_hybrid_threads/) | Threading |
| [13_condvar_basics](homeworks/13_condvar_basics/) | Condition variables |
| [15_advancedmem](homeworks/15_advancedmem/) | Advanced memory exercises |

## Working with the code

Most operating systems exercises expect Linux or WSL, a C/C++ toolchain, and Make. Read the README and Makefile inside the selected exercise before building; this repository contains many independent programs and does not have one root command that compiles all coursework.

The root Makefile is for the **course website**, not the C/C++ exercises. Keep the existing directory layout when using the course documents, because many instructions and links refer to it.

## Previewing the course website

The website uses Ruby, Bundler, Jekyll, and the theme/dependencies declared by `Gemfile` and `beautiful-jekyll-theme.gemspec`.

From the repository root, with Ruby and Bundler available:

```sh
bundle install
bundle exec jekyll serve
```

Open the local address printed by Jekyll. `make serve` invokes the same server command. The root Makefile also provides `background` and `kill` targets for a tmux session named `server`.

The existing `_config.yml` identifies the course term as **Winter 2022–23** and retains upstream instructor, course-service, and repository links. Those links and requirements reflect the original course environment. GitHub Pages publishing additionally depends on the repository's Pages settings.

## Attribution and license

Original instructor attribution, source comments, and supplied solutions are retained. See [LICENSE](LICENSE) for the existing MIT license and copyright notice. This README adds navigation and setup context without replacing the individual course documents.

Former repository name: `csse332_os`.

## Original GitHub Pages guidance

The original README's setup reference is retained below. Its links point to the upstream course repository and the original Pages guidance.

<details>
<summary>Expand the original Markdown, theme, and support notes</summary>

## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/RHIT-CSSE/csse332/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

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

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/RHIT-CSSE/csse332/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

</details>
