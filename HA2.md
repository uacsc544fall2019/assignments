## Homework Assignment 2

Version History: 

- Released, 2019/9/5


Due Thursday September 19, 11:59PM

In this assignment we are:

- Practicing using the d3js library for visualization
- Practicing using a design pattern/framework to handle UI events
- Gaining familiarity reading an interpreting a design study


The artifacts generated should be presented in the HTML pages or LaTeX
documents as described below. No style information should be in the HTML tags
unless explicitly allowed. Do not use HTML tags like `<center>`, `<b>`, or
`<i>` to alter visual appearance.  Programmatically added SVG elements may
have style attributes.

Github Classroom Assignment link: [https://classroom.github.com/a/sUICMxvO](https://classroom.github.com/a/sUICMxvO)

Anything you want graded should be in the repository at the due date in the
`master` (default) branch. Do not forget to `git commit` and `git push` to
`github.com`. You may want to verify through the web client or cloning to
another place to ensure your commits have been made.

### Paper Reading (20 pts)

Read the paper "CerebroVis: Designing an Abstract yet Spatially Contextualized
Cerebral Artery Network Visualization" by Aditeya Pandey et al. and answer the
following questions. These are the same questions from your previous paper
reading assignment.

1. What problem is this paper trying to solve?

2. Why is this problem considered a visualization problem?

3. Why is the problem important?

4. How does this paper contribute to solving the problem? 

5. What approaches are used to construct the contributions?

6. How are the contributions of the paper evaluated or justified? 

7. What do you think are this paper's strengths? 

8. What do you think could be improved about this paper?

9. What future directions do the authors suggest? 

10. What future directions not mentioned in the paper would you suggest?

11. What questions do you have about this paper? For example: Were these things
   you find difficult to understand? Are there details left unanswered? Do you
have philosophical questions regarding some of the points made?

12. How might the concepts or approaches in this paper relate to your course
   project? If you have not yet chosen a course project, give your best guess
with what you are thinking of doing now.

Note: These questions have been adapted from similar guides and assignments by
William G.  Griswold, Premkumar Devanbu, and Michelle Strout.

The results should be submitted as a LaTeX `.tex` file that will compile into
a `.pdf` with the command `pdflatex`. Use the template from the previous
assignment. The name of the `.tex` file should be `reading.tex.`

This portion will be graded on whether you have answered all the questions,
including sub-questions, the thoughtfulness of your answers, and the
readability of your answers.


### Visualization with d3js (80 pts as divided below) 

The directory  is pre-populated with  `ha2.html`, `ha2.css`, `ha2.js`, and
`data.js`. Modify `ha2.html` to put your name in the title. You will modify
`ha2.js` and `ha2.css` in this assignment to implement the below. Do not
change the height and width of the SVGs. 

Use the d3js **version 5** library **and no other**. For the SVGs, do not use
calls to `createElementNS` or `getElementById` etc. You may use these
functions in `createScatterControlsView` if you choose. 

For any scaling you must do, you should use the d3js scale functions (e.g.,
`d3.scaleLinear()`).

#### Bar Chart (15 pts)

Recreate the bar chart showing the grade distribution (yes, a third time!).
This time do it with d3js.  Populate the function `createBarChart` to perform
this operation such that the call to it in `window.addEventListener` works.

#### Scatter Plot (65 pts)

Implement an interactive scatter chart as shown in the movie linked here:
[HA2/videos/HA2-Scatterplot-Functionality.mov](HA2/videos/HA2-Scatterplot-Functionality.mov)

Modify the functions `createScatterModel`,
`createScatterView`,`createScatterControlsView` and `createController` to
implement an interactive scatter plot. Note I have given you the function
`makeSignaller` (from class).

Like in HA1B, the scatter chart encodes four attributes of the Starbucks
dataset from Kaggle. The following enhancements have been made:

- x and y axes have been added
- rather than using `svg:title`, hovering over a point writes a text label at
  the top and adds a 2 pixel red outline to it
- the encoding rule for each channel can be changed via dropdown (`select`) value
- the data points can be filtered by beverage type
- points that appear "grow" into existence, points that disappear "shrink" out
  of existence
- when the points move due to the encoding changing, the axes and points
  appear to animate

The views should be state-less. Do not store information in the views. This
includes state information such as which data point is being hovered.

I recommend building this in stages. Here's one such plan but do it in the
order with which you are most comfortfable:

1. Build the model assuming a static view with no filtering and hovering.

2. Build a mostly-static scatterplot view and test that it works for static
   initializations of  `x`, `y`, `size`, and `color` that you set in the
   model. You will need to update the `window.addEventListneer` call to create
   the model and view.

3. Add in the ability to hover over a point and get the label. This requires
   updating both the model and scatterplot view and creating the controller.
   Test.

4. Make the ControlsView work for a single drop down. First test the drop
   down, then wire it to the rest of the system. Don't worry about the
   transition animations yet.

5. Finish the ControlsView.

6. Add the animations. (d3js transitions)

There are other orders in which you could complete this assignment. For
example, if you want to do the d3js later, you could work on the model,
dropdowns, and controller, testing with `console.log` statements.

##### Grading

Here is a breakdown of grading by functionality. Partially credit may be
assigned for partial completion.

These points assume that state information and data is managed by the model,
views are stateless, and UI events are managed by the controller. Not adhering
to the separation of concerns will result in partial credit for each feature
where the architecture is violated.

- Scatterplot functionality matching HA1B, done in d3js with scales and
  drawing data from the model: 20 pts
- Scatterplot has axes: 10 pts
- Hovering on a circle outlines the circle and draws the label: 10 pts
- Dropdowns are appropriately populated: 5 pts
- Changing a dropdown updates the scatterplot correctly: 15 pts
- When the scatterplot changes:
  - the points that change position are animated: 1 pt
  - the points that appear grow from radius 0: 1 pt
  - the points thtat disappear shrink to radius 0: 1 pt
  - the axes animate to their new values: 2 pts


##### Screenshot

![Screenshot of HA2 Scatterplot when hovering over a point with filtered
data](HA2/images/HA2-Scatterplot.png)
