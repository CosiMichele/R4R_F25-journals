# Learner Log Entry #06

Following the instructions in the main [README.md](README.md/#entries-instructions), fill the following sections as requested, feel free to add as many lines as needed per each section. Please respect the due times for each section.

## Rose, Bud, Thorn

> [!IMPORTANT]
> **Due Wednesday 8th, 11pm**

### Rose

The session on software environments and scripting languages clarified how critical it is to lock down not just your code, but everything around your code—the packages, versions, and environment settings. I appreciated learning concrete tools like Conda for managing isolated environments and how sharing an environment file (.yml or lock file) lets collaborators reproduce exactly the same setup. The side-by-side examples of equivalent scripts in Bash, Python, and R also made clear how different languages can express the same tasks. This helps me see how I might choose a language or environment best suited to my BME projects.

### Thorn

What remains confusing to me is dealing with dependency conflicts (sometimes called “dependency hell”) when two packages require conflicting versions of sub-packages. It’s not always obvious how to resolve such conflicts without breaking something else. I also find it tricky to know when I should freeze an environment versus update it, and how to maintain backward compatibility (so things still run months later). Finally, understanding when to use environment managers like Conda versus built-in language tools (e.g. R’s renv) feels like a judgment call I haven’t yet internalized.

### Bud

I see a lot of value in starting to use environment managers from now on in my coursework and research. I want to create isolated Conda environments for each of my projects so that I don’t accidentally break one project when updating libraries for another. I’m also interested in sharing environment files with classmates or future collaborators so they can replicate my computational work. Over time, I hope to build a habit of exporting and versioning my environments alongside my code, so reproducibility becomes second nature.


---

## Research Application

This module taught me that reproducibility in computational research is not only about the code, but about the computing environment in which the code runs. Even with the same script and input, different package versions or system settings can lead to different outputs. The concept of “software dependency hell” emphasizes how fragile computational workflows can become when environments differ. The solution of using environment managers (like Conda for Python or renv for R) allows projects to be decoupled from the global system setup, and sharing exported environment definitions (e.g. environment.yml, requirements.txt, or renv.lock) lets others reconstruct the same environment on their machines. In biomedical engineering contexts, this is especially important. Suppose I write code for signal processing of ECG data or simulate implant behavior using numerical packages. If I later upgrade a library version, results might subtly shift, which could mislead downstream analysis. By maintaining stable environments, I can guard against those changes. Going forward, I plan to always create a fresh environment for each project, explicitly install only needed packages, and share the environment definition in my repository. That way, others (or even my future self) can reliably reproduce my computational workflows.

> [!IMPORTANT]
> **Due Monday 8th, 11pm**


---

## Cohort meetup discussion

> [!IMPORTANT]

> **Due Thursday 16th, 11am**
