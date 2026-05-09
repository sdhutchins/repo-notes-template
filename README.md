# repo-notes-template 

This is a template I use to keep my notes repo-centric without committing them to git.

## Usage

```bash
copier copy gh:sdhutchins/repo-notes-template .
```

By default, this creates a `_private/` folder with markdown stubs for research
framing, methods, results, tracking, collaboration, references, and glossary
notes. Override the folder name when Copier prompts for `note_folder_name`.

I add this to a global `.gitignore` or one that contains all my GitHub repos.

I also recommend adding `.copier-answers.repo-notes.yml` to that `.gitignore`.

## Updating copied notes

This template writes Copier answers to `.copier-answers.repo-notes.yml` so it can
be updated independently from any other Copier template used by the destination
repo.

```bash
copier update -a .copier-answers.repo-notes.yml
```

## How do you track these notes?

I keep most of my notes in [Joplin](https://joplinapp.org/), and since this is markdown formatted, I have a [script]() 
that just copies these folders to a folder that is aggregated by project.

This allows me to copy this easily into joplin or open the folder in other tools or whatever I want to do.

You could probably find a way to automate or copy this into Joplin (I will solve this later).
