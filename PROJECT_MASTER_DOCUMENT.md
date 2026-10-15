# Farm Robot Path Planning Using A* Algorithms

## 1. Project Objective

Develop and compare A* path-planning algorithms for an agricultural robot navigating through crop rows.

The project focuses on:
1. Understanding the original A* algorithm.
2. Implementing farm-specific path planning.
3. Adding turning penalties.
4. Developing heading-aware A*.
5. Comparing algorithms using quantitative metrics.
6. Documenting methodology, results, limitations, and conclusions.

## 2. Current Project Status

Current phase: Fair comparison of three A* algorithms.

Algorithms:
- Original A*
- Farm A* with turning penalty
- Heading-aware A*

Important: Existing results are preliminary because the algorithms use different grid resolutions and cost models.

## 3. Farm Environment

- Start: (5, 5)
- Goal: (55, 55)
- Field boundaries: approximately x = 0 to 60 and y = 0 to 60
- Crop-row obstacles: x = 15, 30, and 45
- Crop-row extent: approximately y = 10 to 50

Previously used settings:
- Original A* and Farm A*: grid_size = 2, robot_radius = 1
- Heading-aware A*: GRID_SIZE = 1, TURN_WEIGHT = 3

These settings must be checked against the existing implementations before standardizing the experiment.

## 4. Existing Project Files

- a_star.py: Original A* implementation from PythonRobotics.
- a_star_farm.py: Farm-specific A* with a turning penalty.
- compare_farm.py: Comparison script for Original A* and Farm A*.
- a_star_heading.py: Heading-aware A* implementation.

Original repository: PythonRobotics

Previous project directory:
~/PythonRobotics/PathPlanning/AStar

## 5. Preliminary Results

| Metric | Original A* | Farm A* | Heading-aware A* |
|---|---:|---:|---:|
| Path length | 91.11 | 95.80 | 86.53 |
| Number of turns | 12 | 3 | 4 |
| Total turning angle | 540° | 135° | 180° |
| Number of path points | Not recorded | Not recorded | 78 |

These results are preliminary and must not be used to claim that one algorithm is superior.

## 6. Fair Comparison Methodology

Before comparing the algorithms, inspect the existing source code.

Standardize, where applicable:
- Farm map and obstacle placement.
- Grid resolution.
- Start and goal positions.
- Robot collision assumptions.
- Path-length calculation.
- Turn-count and turning-angle calculations.
- Evaluation and reporting procedures.

Preserve the original implementation. Document any required changes before modifying files.

## 7. Computer and Software Environment

Record the following for each computer:
- Computer identifier
- Ubuntu version
- Python version
- Git version
- Repository location
- Dependencies
- Date of verification

Do not assume that the environment is identical across computers.

## 8. Installation and Setup Commands

To be documented after verifying the current computer and repository.

## 9. Algorithm Explanations

To be completed after reviewing the actual implementations.

## 10. Important Code Modifications

Record each modification, the filename, its purpose, and its effect on results.

## 11. Errors and Solutions

Record reproducible errors, their causes, and verified solutions.

## 12. Experimental Results

Record standardized experimental results after the fair comparison is implemented.

## 13. Limitations and Future Improvements

- Existing results use inconsistent experimental settings.
- Collision assumptions must be verified.
- Algorithm performance must be evaluated using a common methodology.
- Additional improvements will be documented as the project develops.

## 14. Current Task

Inspect the existing implementations of:
- a_star.py
- a_star_farm.py
- compare_farm.py
- a_star_heading.py

Then design a fair comparison without unnecessarily replacing working code.

## 15. Next Steps

1. Verify the current computer and software environment.
2. Locate the original PythonRobotics repository and project files.
3. Inspect all four Python files.
4. Identify differences in map settings, grid resolution, collision checking, and cost functions.
5. Design the standardized comparison.
6. Implement and verify the comparison.
7. Record results and update the daily progress log.

## 16. Daily Progress Log

### 2026-10-15
- Created the GitHub repository for working project files.
- Started preparing the master project document.
- Next task: inspect the existing A* implementations and establish fair experimental conditions.
