Variance and standard deviation are two important concepts in statistics that measure the spread or dispersion of a set of data points. Variance quantifies how much the data points deviate from the mean, while standard deviation is the square root of variance and provides a measure of dispersion in the same units as the data. 

This means that the standard deviation will have the same units as the original data, making it easier to interpret. Both variance and standard deviation are used to understand the variability of data, which is crucial for statistical analysis and decision-making.

# Population vs Sample Variance and Standard Deviation

When calculating variance and standard deviation, it's important to distinguish between population and sample data. When we have complete data for an entire population, we use the population variance and standard deviation formulas. However, when we only have a sample of the population, we use the sample formulas to estimate the population parameters. Using $n-1$ instead of $n$ corrects the tendency of the sample variance to underestimate the population variance.

# Variance
Variance measures the average squared deviation of each data point from the mean. The population variance (often denoted as $\sigma^2$) is calculated as:

$$
\sigma^2 &= \frac{1}{N} \sum_{i=1}^{N} (x_i - \mu)^2
& = \frac{1}{N} \sum_{i=1}^{N} x_i^2 - \mu^2
$$

where $N$ is the number of data points in the population, $x_i$ represents each data point from the population, and $\mu$ is the population mean. Either of the two formulas can be used to calculate the population variance, depending on which is more convenient.

The sample variance (denoted as $s^2$) is calculated as:

$$
s^2 &= \frac{1}{n-1} \sum_{i=1}^{n} (x_i - \bar{x})^2
&= \frac{\sum_{i=1}^{n} x_i^2 - n\bar{x}^2}{n-1}
$$

where $n$ is the number of data points in the sample, $x_i$ represents each data point, and $\bar{x}$ is the sample mean. The denominator is $n-1$ instead of $n$ to account for the fact that we are estimating the population variance from a sample.

# Standard Deviation

Standard deviation is the square root of variance and provides a measure of dispersion in the same units as the data. The population standard deviation (denoted as $\sigma$) is calculated as:

$$
\sigma &= \sqrt{\sigma^2}
&= \sqrt{\frac{1}{N} \sum_{i=1}^{N} (x_i - \mu)^2}
&= \sqrt{\frac{1}{N} \sum_{i=1}^{N} x_i^2 - \mu^2}
$$

The sample standard deviation (denoted as $s$) is calculated as:

$$
s &= \sqrt{s^2}
&= \sqrt{\frac{1}{n-1} \sum_{i=1}^{n} (x_i - \bar{x})^2}
&= \sqrt{\frac{\sum_{i=1}^{n} x_i^2 - n\bar{x}^2}{n-1}}
$$

# Examples

Imagine we have measured the heights of 5 people and found them to be 160, 165, 170, 175, and 180 cm. Their mean height is 170 cm. 

Because the data is measured in centimetres, variance is measured in square centimetres ($\text{cm}^2$), while standard deviation is measured in centimetres ($\text{cm}$), the same units as the original data.

## Population Variance and Standard Deviation
We can calculate the variance and standard deviation of that group in isolation by treating it as the complete population.

Population variance:

$$
\sigma^2 &= \frac{1}{5} \left[(160-170)^2 + (165-170)^2 + (170-170)^2 + (175-170)^2 + (180-170)^2\right] \\
&= \frac{1}{5} \left[100 + 25 + 0 + 25 + 100\right] \\
&= \frac{250}{5} \\
&= 50\ \text{cm}^2
$$

Population standard deviation:

$$
\sigma &= \sqrt{\sigma^2} \\
&= \sqrt{50} \\
&\approx 7.071\ \text{cm}
$$

## Sample Variance and Standard Deviation

If we consider the same group of 5 people as a sample from a larger population, we would calculate the sample variance and standard deviation.

Sample variance:

$$
s^2 &= \frac{1}{5-1} \left[(160-170)^2 + (165-170)^2 + (170-170)^2 + (175-170)^2 + (180-170)^2\right] \\
&= \frac{1}{4} \left[100 + 25 + 0 + 25 + 100\right] \\
&= \frac{250}{4} \\
&= 62.5\ \text{cm}^2
$$

Sample standard deviation:

$$
s &= \sqrt{s^2} \\
&= \sqrt{62.5} \\
&\approx 7.906\ \text{cm}
$$

The sample variance and standard deviation are our estimates of the variance and standard deviation of the larger population from which the sample was drawn.