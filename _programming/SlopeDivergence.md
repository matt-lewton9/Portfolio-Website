---
layout: project
title: Initial Slope by Divergence
imgFilename: "slopeMain.png"
when: "Spring 2022"
order: 2
---

<img src="{{ "assets/images/slopeMain.png" | relative_url }}" class="articleImgMain">

I developed an iterative matlab algorithm in my Engineering 132 class to find the initial slope of a dataset. It quantifies a task usually determined by the "eye test" as two numbers, divergence tolerance and error limit, then adjusts those two values iteratively until an acceptable solution is found (No, this is not gradient ascent).

## How It Works

The assignment was to find the initial slope of a hundred datasets that had significant noise and outliers. All of the datasets had the same logarithmic shape, where the slope approaches infinity as time approaches 0 from the left.

My algorithm sets a "divergence tolerance" for the maximum acceptable difference of two point's average slope with the origin. The algorithm iterates through points approaching 0 from the right, finding the difference in average slope between the current selected point and the previous point until it detects that the difference has exceeded the divergence tolerance. 

The selected slope is then checked for error to see if it is acceptable. Normalized error was the average of percent squared error between the slope line and the data points to the left of the selected point, but there are a million ways to characterize error here.

If the error is below a predefined error limit, then the slope is returned as the solution. Else, it continues iterating through points until it reaches time 0, and has run out of points. If this happens, it slightly increases the divergence tolerance and tries again. If, after multiple iterations, the divergence tolerance has been raised to an unacceptable amount, then it resets the divergence tolerance to its original value, and raises the error limit. By increasing these two parameters incrementally, it always returns a good solution.

## Optimization and Efficiency

If you think this program sounds inefficient, you'd be correct, however runtime wasn't a constraint as long as it was reasonable (10^1 minutes), and there are a few optimizations you can make. 

You only have to search in the first 1/8 of the dataset, since that range is where all the solutions will be located. You also can skip points. The final version compared every tenth point, without really affecting accuracy.

There are also a few built in ways to handle data noise and outliers. One, is to return the nth acceptable solution found. This verifies that the algorithm has found a range of acceptable solutions, and hasn't just stumbled on an outlier. The skipping feature mentioned above also helps with noise, as the divergence tolerance is less likely to be tripped by local variations.

In future work, an optimal divergence tolerance and error could be finely honed by machine learning much more accurately and efficiently. However, linearly increasing both of those parameters was adequate to get very accurate results that exceeded what was required for the assignment. 

This project is not on Github due to academic integrity rules, since it was an assignment.
