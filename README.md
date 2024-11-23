# Percolation

Programming Assignment 1 for the Data Structures course  
[Assignment Link](https://ds.cs.rutgers.edu/assignment-percolation/)

## Problem Description

Percolation is a model used to represent the flow of fluid through a porous medium. The problem involves simulating the percolation of water through a grid. Given an n-by-n grid of sites, each site is either open or blocked. The grid percolates if there is a path of open sites connecting any open site in the top row to any open site in the bottom row.

- Each site has a probability *p* of being open.
- The goal is to determine if there is a percolating path, meaning a sequence of connected open sites that connects the top row to the bottom row.

## Approach & Solution

The problem is solved using the **Weighted Quick Union** algorithm, which efficiently handles dynamic connectivity between sites in the grid. The grid is represented using a 2D array, and union-find operations are applied to connect adjacent open sites.

Key details of the solution:

- **Weighted Quick Union** is used to minimize the depth of the tree representing the connected components, improving the time complexity.
- The algorithm runs in **O(n²)** time complexity, where n is the size of the grid.
- The solution checks if there exists a path from any open site in the top row to any open site in the bottom row.

## How It Works

- A 2D array represents the grid, where each cell can either be open or blocked.
- Union-find is used to efficiently check if any open site in the top row is connected to an open site in the bottom row.
- If such a path exists, the system percolates.

## Key Features

- **Weighted Quick Union** for efficient dynamic connectivity.
- 2D array representation of the grid.
- Supports random site openings with a given probability p.
- Determines if the system percolates based on the given configuration.
