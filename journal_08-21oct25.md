# Learner Log Entry #08

Following the instructions in the main [README.md](README.md/#entries-instructions), fill the following sections as requested, feel free to add as many lines as needed per each section. Please respect the due times for each section.

## Rose, Bud, Thorn

> [!IMPORTANT]
> **Due Wednesday 22nd, 11pm**

### Rose

I found the overview of the high-performance computing (HPC) environment very helpful: the section “A 10,000 ft View of the HPC” gave a clear explanation of how cluster systems are organised and how user access works. 
Learning about how the workload manager SLURM works (job queues, resources, partitions) directly connects with the kind of batch analysis tasks I anticipate in BME lab work (e.g., processing large imaging datasets). 
The explanation of using Apptainer (formerly Singularity) for containerised execution on HPC was particularly relevant — as in my lab we often struggle with software version conflicts, and seeing that Apptainer allows rootless containers is a relief.

### Thorn

Some of the instructions assume familiarity with Linux terminal commands, modules, job-submission scripts, and cluster operations. As someone whose background is more in biomedical applications than computational systems, I felt slow getting up to speed on commands like sbatch, squeue, module load, etc.
The distinction between interactive node usage versus batch job submission, and when to pick which, wasn’t fully intuitive to me yet—especially how it relates to our typical lab workflows (data acquisition vs post-processing).
While the material mentions storage quotas (home folder, group folder, large research disk) and queue times, I worry about how realistic the wait-times will be for my BME data workflows (for example, if I need to run a heavy simulation or imaging pipeline) and whether I’ll be able to anticipate resource bottlenecks ahead of time.

### Bud

I want to try submitting a small interactive job on the HPC to test how it works firsthand, for example launching an interactive node with modest resources to run a MATLAB or Python-based signal-processing script from our lab.
I’m interested in containerising one of our imaging-analysis pipelines (for example, a Python-OpenCV or imageJ workflow) using Apptainer and running it on the HPC, thereby integrating reproducibility with the computing power of the cluster.
I hope to document a “cheat sheet” of the key commands (login, module, job submission, resource checking) tailored to BME lab tasks — this could help my lab-mates (many of whom are less computational) adopt HPC tools more confidently.

---

## Research Application

As a Biomedical Engineering undergraduate working in a lab environment, I engage in data-driven workflows (e.g., acquisition of bio-signals, image processing of cell cultures, finite-element simulations of biomechanics). The HPC module provides a direct pathway to elevate those workflows in the following ways:
Large-scale Data Processing for BME Labs
In our lab, we occasionally accumulate high-resolution microscopy image stacks or long‐duration bio‐signal recordings. By leveraging the HPC cluster (via SLURM) I can run scripts that would otherwise take many hours on a regular workstation. For example, I can submit a batch job that processes hundreds of image files using Python/OpenCV or MATLAB, thus freeing up my local machine and accelerating turnaround.
Simulation & Modeling Workflows
Biomechanical modeling often demands large RAM and CPU resources (or even GPUs). Using the HPC, I can choose an appropriate cluster (e.g., “Puma” vs “Ocelote” as listed in the lesson) depending on how intensive the task is. 
 I plan to create a SLURM job script specifying memory (--mem), cores (--cpus-per-task), and time limits that match my simulation needs.
Containerised Reproducibility for Lab Experiments
To ensure that our lab software environment remains consistent across students and over time, I will build an Apptainer container containing all the dependencies (e.g., Python 3.x, NumPy, SciPy, OpenCV or MATLAB runtime) and execute it on the HPC. This will allow me to share the container with fellow lab-mates or retain the environment for future reuse.
Collaboration and Scalability
When collaborating with others (e.g., undergraduate peers or graduate students), sharing a container plus a standardized HPC job submission script will ensure everyone uses identical setups. This reduces “it worked on my machine” problems, especially important when analyzing biomedical data that might vary by software version.
Workflow for My Current Lab Project
Specifically, for my current lab work I plan to:
Containerise the script that processes EMG signals (filtering, Fourier transform, feature extraction).
Submit that container as a job on the HPC with a SLURM script (e.g., requesting 4 cores, 8 GB memory, 1 hour runtime) so that I can process multiple datasets in parallel.
Archive the Apptainer .sif image and the SLURM script as part of my lab report appendix to demonstrate reproducibility.

> [!IMPORTANT]
> **Due Monday 20th, 11pm**


---

## Cohort meetup discussion

> [!IMPORTANT]

> **Due Thursday 30th, 11am**
