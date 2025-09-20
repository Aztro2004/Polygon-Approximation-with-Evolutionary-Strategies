# PPolygon-Approximation-with-Evolutionary-Strategies

Final proyect for the class of Evolutionary Computing at UNAM ENES Unidad Morelia.

## Author

Diego Maldonado Castro: diegomaldonadocastro1805@gmail.com

## Introduction

This project implements (μ + λ) evolutionary algorithm for 3D shape approximation using numpy.



## Features

- Evolutionary strategy: (μ + λ) selection
- Crossover and mutation of 3D shapes (points in space)
- Fitness function using 3D IoU (Intersection over Union)
- Output of best individual per run



## Algorithm Overview

The algorithm maintains a population of 3D point clouds (individuals), which are evolved over generations via:
- **Crossover**: Combining traits from two parents.
- **Mutation**: Random variation within defined bounds.
- **Fitness Evaluation**: How well the point cloud matches a target shape through its convexhall.

MPI is used to parallelize the fitness evaluation step, significantly improving runtime on multi-core systems.

## Results

![evolution](https://github.com/user-attachments/assets/e90a3ba1-f013-4e77-b313-6ca254c67cb3)

Example of a 200 point individual approximating a sphere.

## Dependencies

