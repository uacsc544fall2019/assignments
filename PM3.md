## Project Milestone 3

Version History: 

- Revision re: PM3.pdf, 2019/10/31 (I will still accept P32.pdf too)
- Revision re: code, 2019/10/27
- Released, 2019/10/14


Due Thursday October 31, 11:59PM

In this milestone we are:

- Reporting on our progress with the project
- Creating artifacts of our progress on the project, e.g., code 
- Assessing changes made since our previous milestone
- Correcting deficiencies in our previous milestones
- Getting more practice with LaTeX

Create a repository for this milestone at this following Github Classroom
link: [https://classroom.github.com/g/N6qront9](https://classroom.github.com/g/N6qront9).

All material you want graded should be in that folder at the deadline. All the
files needed to compile your document should be in that folder. There is a
geometric penalty associated with repeated failure to follow these
instructions. **NO Auxilliary files should be in that folder. Do not include
PM3.pdf, PM3.aux, etc.** 

Continue to use the LaTeX files required to format an IEEE VGTC-style
document. Like in PM2, I am not providing the rest of the files. You
will likely want to copy `PM2.tex` from last milestone and adapt it to
the requirements below.

There should be a `PM3.tex` file that compiles into a `PM3.pdf` file when I
type `make`.

Create a folder named `Project` in your repository. This folder should include
code and any other files required to eventually run your project. It may also
include data for data-collection-centric projects.

Your PM3 report should include several sections described below. Also, see my
comments in Project Milestone 2 for any additional information I expect to see
in this milestone.

## Movie

Create a short `PM3.mp4` or `PM3.mov` file demonstrating your technical
progress on the visualization and the interactions supported. It should show
how the visualization is launched and what is shown. The movie should be no
longer than three minutes. 

The video should include some description of what is going on. This can be
done in a separate text file (`.tex`, `.txt`, or `.md`) or can be done through
voice over. If a file is used, please name it `pm3-movie`. If no such file is
found, audio will be assumed.


## Report

Your PM3 report should include several sections:

#### Abstract

Briefly describe your project and contributions you have made for this
miletsone.


#### Section: Overview

Create a top level section called `Overview`. In this section, describe the
overall goal of your project -- what overarching problem is it trying to help
solve (not necessarily a visualization problem) and then what is the
visualization aspect of that problem that your project entails. This should be
like the section you did for PM2, but updated with any changes made since the
last milestone.

At the end of this section, summarize what work was completed for this milestone. 


#### Section: Technical Progress 

Create a top level section called `Technical Progress`. In this section,
describe what progress has been made. Such progress may include (1)
understanding any systems with which you will use or integrate, (2) coding in
service of the goals of your project (e.g., data reader, views, etc), (3)
proof of concepts, and (4) data collection. **In this milestone, technical
progress regarding reading in the data and creating an initial view is
required at a minimum for visualization design projects. For each
contribution, create a separate subsection under this section to describe
it.**

In your descriptions, you may refer to the movie to help explain the progress.
If you progress includes visualizations or partially done visualizations, use
figures to describe and demonstrate the progress made. Describe the
technologies (e.g., languages, libraries, platforms) used to support your
progress.

If the progress includes a better understanding of how the systems work, use
this section to describe that understanding for others. For example, if your
project requires understanding multiple modules interact, describe how those
modules interact here, as if you were writing up that knowledge for a final
paper.

Proof of concepts may include code that will not be part of your final
project, but demonstrate that some technical piece of your project will work.
For example, if you plan to rely on a third party library, it could be a short
script demonstrating that library works. 

Code associated with the contribution, including proof of concepts, should be
available in the Project directory at the top level of your repository. Some
of it is required to run. **Instructions for how to get it to run must be
included in the Project directory in a file called README.md. Revision 2019/10/27: If y ou are dealing with huge data, do not upload huge data to repository. If you can include a toy dataset, do that instead. Otherwise, email me and we'll work something out like a live demo or extended movie.** 

If you collected data for the visualization of this milestone, please describe
your data collection efforts here. What did you do to collect the data? Is
there still more that you have to do? Data collected to support the task
abstraction or design should be described in those respective sections.


#### Section: Refinement from Previous Milestone

Create a top level section called `Refinement from Previous Milestones`. If
you were told to refine any subsection of the previous milestone, included the
refined version of that section as a subsection here. If you were not told to
refine any section, simply write `None requested.` 

**You only need to refine what is listed next to "Refinements needed for
PM3."** Help for how you may refine could be found in the 'Where you missed
points' sections. However, you do not need to refine every place you missed
points.


#### Section: Schedule

Create a top level section called `Schedule`. In this section, describe what
parts of your proposed PM3 goals have been met. Then describe which goals were
not met and an explanation of what choices or unexpected challenges led them
not to be met.

Describe what work will be done for the next two milestones, in light of
what was done for this milestone. 



