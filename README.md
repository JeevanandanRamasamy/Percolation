# Percolation

Programming Assignment 1 for Data Structures course

http://coursera.cs.princeton.edu/algs4/assignments/percolation.html

## Problem

Write a program to estimate the value of the percolation threshold via Monte Carlo simulation.

Given a composite systems comprised of randomly distributed insulating and metallic materials: what fraction of the materials need to be metallic so that the composite system is an electrical conductor? Given a porous landscape with water on the surface (or oil below), under what conditions will the water be able to drain through to the bottom (or the oil to gush through to the surface)? 

In a famous scientific problem, researchers are interested in the following question: if sites are independently set to be open with probability p (and therefore blocked with probability 1 − p), what is the probability that the system percolates? When p equals 0, the system does not percolate; when p equals 1, the system percolates.

## Solution

Found whether the water percolates using Weighted Quick Union and a 2-D array structure in n-squared time complexity.
