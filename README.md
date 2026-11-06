# quantum-wire-poisson-fem

University course project (work in progress).

The goal is to compute the electrostatic confinement potential in a GaAs
T-shaped structure surrounded by metal gates, and later use it to find
bound electron states in a quantum wire.

## Status

Early stage. I'm still working on this and learning as I go.

- [ ] Part 1: solve the Laplace equation for the potential φ(x, y)
- [ ] Part 2: bound states in the resulting potential (not released yet)

## Problem

The structure is uniform in the z direction, so the problem is 2D.
The bottom electrode is at potential 0, the top electrode at V. Far from the middle, the potential should look like that of a flat capacitor.

We solve

    -∇²φ = 0

with a finite element method on a mesh of 80 square elements
(369 nodes, element side a = 6.25 nm).

## Input data

The node positions and local->global numbering come from files provided
by the course instructor. They are included in the repo.

## Tech

Python, NumPy, Matplotlib (Jupyter notebook).

## Notes

This is a student project, work in progress.