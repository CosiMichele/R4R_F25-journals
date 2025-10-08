# Learner Log Entry #03

Following the instructions in the main [README.md](README.md/#entries-instructions), fill the following sections as requested, feel free to add as many lines as needed per each section. Please respect the due times for each section.

## Rose, Bud, Thorn

> [!IMPORTANT]
> **Due Wednesday 17th, 11pm**

### Rose

This lesson opened my eyes to how powerful the command line (CLI / Unix shell) can be—even for things I already do in my lab courses. Even though my work is mostly structured around lab reports and data tables, being able to use terminal commands could speed things up and make file operations more precise than using click-and-drag interfaces.
For example: when I have a folder of data files from multiple runs of an experiment, instead of manually renaming or moving them in a file explorer, I could use commands like mv, cp, or rm to reorganize everything in seconds. Or use ls -a -l to quickly see file permissions, sizes, and hidden files rather than clicking through properties. The reading also showed how to automate common tasks with shell scripts, which seems very promising — I can imagine writing a small .sh script to clean or preprocess my dataset files before analysis.

### Thorn

I ran into some confusion when it came to scripting, specifically, how to combine commands and variables inside a .sh script. The reading gives an example (find a file, navigate, count keywords, append logs, etc.), but it’s a lot to digest in one go. I’m not yet comfortable with things like $(find . -name "haiku.txt") or embedding if statements or loops.
Also, since I don’t yet have big data pipelines in my coursework, it’s not obvious how to scale these practices for my small lab datasets. Should I always write a shell script for each lab? Or only for more complex tasks? That decision isn’t clear yet.

### Bud

One concrete idea is to start mini scripts for recurring tasks in my coursework. For example, if after each lab I have to:
rename files into a standardized pattern (e.g. experiment1_run2.csv),
move files into appropriate folders (e.g. raw/, processed/),
generate backups,
then I can write a short .sh script that automates those steps. Over time, I’ll build confidence in script writing and understand when such automation is beneficial.
Also, I want to practice using basic commands daily. Even something as simple as navigating directories with cd, listing files, creating a folder with mkdir, or copying with cp — doing that instead of always using the GUI will help me internalize the syntax.


---

## Research Application

Here’s how I could apply these ideas right now, in my lab / coursework environment:
Faster file ops: Instead of manually dragging and dropping many files, I can use mv, cp, rm, mkdir from the terminal. This is especially helpful when working in remote environments (e.g. on a server or remote machine).
Consistent naming / directory structure: I’ll adopt a naming scheme (no spaces, use underscores or hyphens) and enforce it via shell commands, so my directories don’t get messy.
Automation via scripts: For multi-step routines (e.g. copying, renaming, backup), I can package them into a .sh script. So instead of executing each step manually, I run ./process_lab.sh and let the computer do the work.
Reproducibility and transparency: In writing reports, I can show (or share) the scripts I used to process raw data. That way, someone else reading my work could execute the same commands and see exactly how I transformed the data.
Scalable growth: As assignments or projects grow in complexity, these scripts will scale better than manual steps. What takes 10 minutes manually might take 10 seconds via script.

> [!IMPORTANT]
> **Due Monday 22nd, 11pm**


---

## Cohort meetup discussion

> [!IMPORTANT]

> **Due Thursday 25th, 11am**
