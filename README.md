# simple-ST

A minimalist, function-based Python pipeline for segmentation and spot detection in spatial microscopy images.

## Design philosophy

This project is intentionally simple.

- Function-first: the pipeline is built around a small number of high-level functions
- Folder-based I/O: input and output are plain directories, not complex data objects
- Minimal abstraction: no workflow engines, no heavy frameworks
- Research-oriented: readable code, editable parameters, reproducible results

If a task can be solved with a function, it should not require anything more.

## What this pipeline does

Given a folder of microscopy images, the pipeline can:

1. Load images from disk
2. Perform basic preprocessing
3. Segment objects or regions
4. Detect spatial spots (e.g. RNA spots)
5. Save processed images and result tables to an output folder

Each step is configurable via function parameters.

## Installation

Install required dependencies first:

```bash
pip install numpy scipy scikit-image pandas tifffile
