# PyP

This is a Python Package containing Guassian Distribution implementation.

## Installation

To install the package, run the following command in your terminal:

```bash
pip3 install .
```

## Usage

After installation, you can use the package by starting the Python interpreter from the terminal:

```bash
python3
```

Within the Python interpreter, you can use the Gaussian distribution class as follows:

```python
from distributions import Gaussian

# Create a Gaussian distribution object with a mean of 25 and a standard deviation of 2
gaussian_one = Gaussian(25, 2)

# Access the mean of the Gaussian distribution
print(gaussian_one.mean)

# Add two Gaussian distributions
gaussian_two = gaussian_one + gaussian_one
print(gaussian_two.mean)
```

## Features

- Create Gaussian distribution objects

- Access the mean and standard deviation

- Add two Gaussian distributions

## Requirements

- Python 3.x

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
