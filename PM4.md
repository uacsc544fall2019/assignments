## Project Milestone 4

Version History: 

- Released, 2018/11/3


Due Thursday November 21, 11:59PM

In this milestone we are:

- Reporting on our progress implementing the first full prototype of our
  project
- Creating artifacts of our progress on the project, e.g., code in the
  progress directory
- Tying the work on our project to the previous milestones. 
- Assessing changes made since our previous milestone
- Getting more practice with LaTeX

Create a repository for this milestone at this following Github Classroom
link: [https://classroom.github.com/g/KEII5mJD](https://classroom.github.com/g/KEII5mJD).

All material you want graded should be in that folder at the deadline. All the
files needed to compile your document should be in that folder. There is a
geometric penalty associated with repeated failure to follow these
instructions. **NO Auxilliary files should be committed to that folder. Do not
include PM4.pdf, PM4.aux, etc.** 

Continue to use the LaTeX files required to format an IEEE VGTC-style
document. As in PM2 and PM3, I am not providing the rest of the files. You
will likely want to copy files from you last milestone and adapt it to the
requirements below.

There should be a `PM4.tex` file that compiles into a `PM4.pdf` file when I
type `make`. Include the updated Makefile. Additionally, there should be a
short movie demonstrating your functioning prototype.

As with PM3, the code and any other files required to run your project should
be available in the `Project` directory unless we have discussed ahead of time
an alternative due to very large data, proprietary software, or similar.

## Movie

Create a short `PM4.mp4` or `PM4.mov` file demonstrating your technical
progress on the visualization and the interactions supported. It should show
how the visualization is launched and what is shown. The movie should be no
longer than three minutes. 

The video should include some description of what is going on. This can be
done in a separate text file (`.tex`, `.txt`, or `.md`) or can be done through
voice over. If a file is used, please name it `pm4-movie`. If no such file is
found, audio will be assumed.


## Report

Your PM4 report should include several sections:

#### Abstract

Briefly describe your project and contributions you have made for this
milestone.


#### Section: Overview

Create a top level section called `Overview`. In this section, describe the
overall goal of your project -- what overarching problem is it trying to help
solve (not necessarily a visualization problem) and then what is the
visualization aspect of that problem that your project entails. This should be
like the section you did for PM3, but updated with any changes made since the
last milestone. **Note: You may have changed the overall goals for this
semester in the previously milestones. If this changes the overview, that
should be updated to reflect it.**

Then, summarize what work was completed for this milestone. 


#### Section: Visualization 

**This section is for Visualization Design Projects.**

Create a top level section called `Visualization`. In this section, describe
your visualization as if you were presenting it to an academic audience of
visualization researchers. It should describe:

- the design in terms of views and supported interactions 
- the design choices and the rationale behind them
- how the design relates to the data and task abstractions

Use figures to describe your visualization. 

You may refer back to your PM2 or PM3 for the data and task abstraction or you
may copy those sections from the previous milestones in a section called `Data
and Task Analysis`. Use the LaTeX `\ref` command to refer to figures and
sections or subsections.

If you created or modified an algorithm or architecture in support of your
project, also document it in this section. The audience here is other
researchers who may want to learn or copy from your modifications or design.

I recommend creating subsections for the separate views and features to
enhance readability.

DO NOT report on work that you have not completed in this section. The
`Visualization` section should only report on what what your visualization
does, not future work or plans. **As stated in Lecture1, the submitted
visualization should be commensurate with group size.**

Create a subsection called `Implementation`. In this section, describe the
technologies you used, including programming languages, libraries, and
platforms. 

Unless we have discussed an alternative for your project, code associated with
the contribution, including proof of concepts and work in progress described
in the next section, should be available in a directory called `Project.`The
code described in this section is required to run.  **Instructions for how to
get it to run must be included in the Project directory in a file called
README.md**

#### Section: Study Design

**This section is for projects conducting some kind of study.** 

Create a top level section called `Study Design`. In this section, describe
your study design as if you were presenting it to an academic audience of
visualization researchers. It should describe:

- the design in terms of variables, conditions, and format
- the design choices and the rationale 

Use figures if applicable. 

You may refer back to your previous project milestones for your rationale or
to prior work. You can copy a section from a previous milestone if it makes
sense or use the LaTeX `\ref` command to refer to figures and sections or
subsections.

If you created or modified an algorithm or architecture in support of your
project, also document it in this section. The audience here is other
researchers who may want to learn or copy from your modifications or design.

I recommend creating subsections for the major points to enhance readability.

If you have results, create a new top level section called `Results` that
reports on those results. You may want to create another top level sectio
called `Discussion` that discusses those results. You want to keep the hard
facts of `Results` separate from any opinions/interpreations in `Discussion.`

DO NOT report on work that you have not completed in this section. The
`Visualization` section should only report on what what your visualization
does, not future work or plans. **As stated in Lecture1, the submitted
visualization should be commensurate with group size.**

Create a subsection called `Implementation`. In this section, describe the
technologies you used, including programming languages, libraries, and
platforms. 

Unless we have discussed an alternative for your project, code associated with
the contribution, including proof of concepts and work in progress described
in the next section, should be available in a directory called `Project.`The
code described in this section is required to run.  **Instructions for how to
get it to run must be included in the Project directory in a file called
README.md**

#### Section: Process

In this section, describe the process you went through in implementing PM4.
What went more smoothly than expected? What proved to be more difficult? What
work was done that was not reflected in the `Visualization` or other technical
section? 


#### Section: Schedule

Create a top level section called `Schedule`. In this section, describe what
parts of your proposed PM4 goals have been met. Then describe which goals were
not met and an explanation of what choices or unexpected challenges led them
not to be met.

Describe what work will be done in the final milestone in light of what was
done for this milestone.



