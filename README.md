# Rubik's Cube Solver

This project is a comprehensive Rubik's Cube solver that includes three different representations of the cube: 3D, 1D, and bitboard. We implement various search algorithms such as Breadth-First Search (BFS), Depth-First Search (DFS), Iterative Deepening Depth-First Search (IDDFS), and Iterative Deepening A* (IDA*) to solve the cube.

## Table of Contents

1. [Introduction](#introduction)
2. [Cube Representations](#cube-representations)
    - [3D Representation](#3d-representation)
    - [1D Representation](#1d-representation)
    - [Bitboard Representation](#bitboard-representation)
3. [Search Algorithms](#search-algorithms)
    - [Breadth-First Search (BFS)](#breadth-first-search-bfs)
    - [Depth-First Search (DFS)](#depth-first-search-dfs)
    - [Iterative Deepening Depth-First Search (IDDFS)](#iterative-deepening-depth-first-search-iddfs)
    - [Iterative Deepening A* (IDA*)](#iterative-deepening-astar-ida)

## Introduction

This project provides an implementation of a Rubik's Cube solver that supports multiple cube representations and search algorithms. It aims to offer a flexible and efficient way to solve the Rubik's Cube, catering to various computational preferences and requirements.

## Cube Representations

### 3D Representation

The 3D representation mimics the physical structure of the Rubik's Cube. It uses a 3x3x3 matrix to represent the cube's state, allowing for intuitive visualization and manipulation of the cube's faces and turns.

### 1D Representation

The 1D representation flattens the cube into a single array. This format is more memory-efficient than the 3D representation and simplifies certain operations, such as indexing and slicing.

### Bitboard Representation

The bitboard representation encodes the cube's state into a series of bit fields. This method leverages bitwise operations for fast and compact state manipulation, making it suitable for performance-critical applications.

## Search Algorithms

### Breadth-First Search (BFS)

BFS explores all possible states level by level. It guarantees finding the shortest solution but can be memory-intensive due to its extensive use of the queue data structure.

### Depth-First Search (DFS)

DFS explores as far as possible along each branch before backtracking. It uses less memory compared to BFS but does not guarantee the shortest solution.

### Iterative Deepening Depth-First Search (IDDFS)

IDDFS combines the space efficiency of DFS with the optimality of BFS. It performs DFS to increasing depths, ensuring that the shortest solution is found with manageable memory usage.

### Iterative Deepening A* (IDA*)

IDA* is an extension of IDDFS that uses heuristics to guide the search. It iteratively deepens the search with a cost threshold, improving efficiency by pruning unlikely paths.


