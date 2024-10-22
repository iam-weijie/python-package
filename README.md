# pb-distr

This is a Python Package containing implementations of Gaussian and Binomial Distributions.

## Installation

To install the package, run the following command in your terminal:

```bash
pip3 install pb-distr
```

## Usage

After installation, you can use the package by starting the Python interpreter from the terminal:

```bash
python3
```

Within the Python interpreter, you can use the distributions as follows:

### Gaussian Distribution

```python
from pb_distr import Gaussian

# Example 1: Create a Gaussian distribution object with default mean 0 and standard deviation 1
gaussian_one = Gaussian()

# Example 2: Read data from a file and calculate mean and standard deviation
gaussian_one.read_data_file('data.txt')
print(gaussian_one.mean)
print(gaussian_one.stdev)

# Plot a histogram and the probability density function (pdf) of the Gaussian distribution
gaussian_one.plot_histogram_pdf()

# Example 3: Add two Gaussian distributions
gaussian_two = Gaussian(5, 2)
combined_distribution = gaussian_one + gaussian_two
print(combined_distribution.mean)
print(combined_distribution.stdev)
```

### Binomial Distribution

```python
from pb_distr import Binomial

# Example 1: Create a Binomial distribution object with probability 0.5 and 20 trials
binomial_one = Binomial(0.5, 20)

# Example 2: Read data from a file and calculate mean and standard deviation
binomial_one.read_data_file('binomial_data.txt')
print(binomial_one.mean)
print(binomial_one.stdev)

# Plot a bar chart and the probability density function (pdf) of the Binomial distribution
binomial_one.plot_bar_pdf()

# Example 3: Add two Binomial distributions with the same probability
binomial_two = Binomial(0.5, 10)
combined_binomial = binomial_one + binomial_two
print(combined_binomial.p)
print(combined_binomial.n)
```

## Features

- Create Gaussian distribution objects

- Create Binomial distribution objects

- Read data from a file for both Gaussian and Binomial distributions

- Access the mean and standard deviation of distributions

- Plot histograms and probability density functions (pdf) for distributions

- Add two distributions of the same type

## Requirements

- Python 3.x

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- This package is developed under the guidance and course material of Unity's AI Programming with Python.

- It is inspired by the need to easily create and manipulate Gaussian and Binomial distributions in Python.
