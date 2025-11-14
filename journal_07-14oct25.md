# Learner Log Entry #07

Following the instructions in the main [README.md](README.md/#entries-instructions), fill the following sections as requested, feel free to add as many lines as needed per each section. Please respect the due times for each section.

## Rose, Bud, Thorn

> [!IMPORTANT]
> **Due Wednesday 15th, 11pm**

### Rose

I finally understood how containers can simplify lab software management. In my BME labs, we often have to install multiple versions of MATLAB, ImageJ, or Python packages like NumPy and OpenCV. Using containers would completely eliminate compatibility problems between lab computers. The hands-on example in the README made it clear how to build and run a container image step by step. It helped me visualize how researchers can “package” an entire lab setup for reproducibility. I liked that containers provide a consistent environment, that’s especially useful in data analysis labs, where different operating systems can cause code to behave differently.

### Thorn

It was confusing at first to differentiate between Docker images, containers, and virtual machines since all seem to “isolate” environments. The README assumed some background knowledge that I didn’t fully have, so I had to read external resources.
My laptop had trouble pulling one of the example images because of permission issues with Docker Desktop. This slowed me down and made me realize how technical setup can become a real barrier in wet-lab or undergrad courses.
Some of the example code wasn’t directly biomedical-related, so it took extra effort to think about how it would apply to my field (e.g., imaging analysis, bio-signal processing, etc.).

### Bud

I want to try building my own simple container for a BME data analysis workflow, like using Python with SciPy and Matplotlib to analyze a muscle EMG signal.
I’d like to containerize one of our lab simulation tools (maybe COMSOL or a basic MATLAB script) so future students can reproduce the same simulation environment easily.
In the long term, I’m curious about whether containers could help us share lab protocols that require both coding and specific hardware drivers (like microcontrollers or sensors).

---

## Research Application

As a Biomedical Engineering undergraduate, most of my research and lab work involves running small data analysis scripts or simulation models that depend on specific software setups. Containers could make this process far more reproducible and less time-consuming for students and instructors alike.
Here’s how I’d apply containerization in a BME research or lab context:
Reproducible Computational Labs
In our data acquisition labs, we use Python-based tools for processing biological signals. I could create a container that includes Python, Jupyter Notebook, NumPy, and SciPy with preset versions — ensuring every student runs identical software environments during experiments.
Image Analysis for Cell or Tissue Studies
For example, if we run ImageJ macros or OpenCV-based scripts to analyze microscopy images, a container would guarantee that all dependencies and plugins are pre-installed. This prevents “it worked on one computer but not another” issues.
Collaborative Research Projects
When working on group projects or senior design prototypes, containers could make collaboration smoother. We could share a container image that includes both our simulation software and data preprocessing scripts — allowing everyone to test under the same conditions.
Long-Term Reproducibility
If I later revisit a project (for example, to publish or expand it), I could re-run the same container and recreate the results exactly. That’s a huge advantage in scientific reproducibility — something especially important in biomedical research involving sensitive data.
Potential Future Experiment
I’d like to explore combining containerization with sensor-based experiments. For instance, a containerized Python script could interface with an Arduino or NI DAQ device to collect real-time physiological data — giving each lab station a standardized software setup.

> [!IMPORTANT]
> **Due Monday 13th, 11pm**


---

## Cohort meetup discussion

> [!IMPORTANT]

> **No Cohort discussion due this week**
