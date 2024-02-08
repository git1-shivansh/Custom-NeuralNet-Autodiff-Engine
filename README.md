# Custom Neural Network Components in Python

## Introduction
This repository contains Python code for implementing basic neural network components from scratch. It includes classes for values with automatic differentiation, neurons, and layers, along with code for mathematical operations and graph visualization.

## Installation
To use this code, you will need Python installed on your system along with the following packages:
- `math`
- `numpy`
- `matplotlib`
- `graphviz`
- `torch`

You can install these packages using pip:
```bash
pip install numpy matplotlib graphviz torch
```

## Usage
To use the components in this repository, import the necessary classes and functions into your Python script. Here's a simple example to get started:

```python
from custom_neural_net import Value, Neuron, Layer  # Assuming your file is named custom_neural_net.py

# Example usage
x = [2.0, 3.0]
n = Layer(2, 3)
output = n(x)
print(output)
```

## Code Description
- `Value`: A class that represents a scalar in our computational graph and supports automatic differentiation.
- `Neuron`: Represents a neuron in a neural network.
- `Layer`: Represents a layer in a neural network, consisting of multiple neurons.
- Mathematical operations: The code includes implementations for basic mathematical operations like addition, multiplication, and trigonometric functions.

## Visualizing Computational Graphs
The code includes functionality to visualize computational graphs using `graphviz`. Here's how you can use it:

```python
from custom_neural_net import Value, draw_dot

# Create some Values
a = Value(2.0)
b = Value(3.0)

# Perform operations
c = a + b

# Visualize the graph
graph = draw_dot(c)
graph.render('output', view=True)  # Saves and opens the graph image
```

## Contributing
Contributions to this project are welcome. Please feel free to fork the repository, make changes, and submit a pull request.

