# Norminette in GitHub Actions

## What is GitHub actions?

Github Actions enables you to create custom software development lifecycle workflows directly in your Github repository. These workflows are made out of different tasks so-called actions that can be run automatically on certain events - in this case, run Norminette in your repository when a push or pull request occurs. 

## Why you should use it?

Because it's cool and you can include a nice badge in your project repository to impress your friends (![Norminette](https://github.com/caio-vinicius/Philosophers/actions/workflows/main.yaml/badge.svg)). Also, how a continuous integration tool works, which you're sure to see in your developer career. GitHub Actions is simple and free, you can simply use it by adding a few files to your repository and automating a lot of things - it's a bunch of powerful Azure machines!

## How to use it!

1. Identify the repository you want to use this Workflow.

2. Access the repository folder in your machine.

3. In the path of your repository, clone this repository:

```bash
$ git clone git@github.com:caio-vinicius/norminette-github-actions.git
```

4. Create a folder `.github` with another folder `workflows` inside it.

```bash
$ mkdir -p .github/workflows
```

5. Move the `main.yaml` file to `.github/workflows` folder.

```bash
$ mv norminette-github-actions/main.yaml .github/workflows
```

6. Commit it to your remote repository. 

7. Now, to run it, you need to make changes in a .h or .c file in your repository and commit it. Since the `on` directive inside the `main.yaml` is specifying that will only trigger when these files changed.

8. Done!

## How add the nice badge in markdown file!

This: ![Norminette](https://github.com/caio-vinicius/Philosophers/actions/workflows/main.yaml/badge.svg)

To add it:

1. Copy

`![example workflow](https://github.com/<OWNER>/<REPOSITORY>/actions/workflows/main.yaml/badge.svg)`

2. Replace OWNER and REPOSITORY with yours:

`![example workflow](https://github.com/niceguy/nicerepo/actions/workflows/main.yaml/badge.svg)`

3. Paste in your markdown file.

4. Done!
