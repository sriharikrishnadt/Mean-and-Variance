#  Mean and variance of a discrete  distribution


# Aim : 

To find mean and variance of arrival of objects from the feeder using probability distribution


# Software required :  

Python and Visual components tool

# Theory:

The expectation or the mean of a discrete random variable is a weighted average of all possible
values of the random variable. The weights are the probabilities associated with the corresponding values. 
It is calculated as,

![image](https://user-images.githubusercontent.com/103921593/192938463-e34177f4-f188-48a0-bda2-8f6d1d660ed2.png)

The variance of a random variable shows the variability or the scatterings of the random variables.
It shows the distance of a random variable from its mean. It is calcualted as

![image](https://user-images.githubusercontent.com/103921593/192938695-99fedc01-34d5-4d36-84df-5880e766ed0c.png)


# Procedure :

1. Construct frequency distribution for the data

2. Find the  probability distribution from frequency distribution.

3. Calculate mean using 
   
   ![image](https://user-images.githubusercontent.com/103921593/192940431-03b81777-c54d-4286-b4f4-82dfe7666b4c.png)

4. Find  
   
      ![image](https://user-images.githubusercontent.com/103921593/192940255-2d9dd746-6875-4a6d-877b-6da6cdb96ab1.png)

5.  Calculate variance using 
  
      ![image](https://user-images.githubusercontent.com/103921593/192942852-913550a9-fabe-4a55-b956-0487b18bbd97.png)


# Experiment :

![image](https://user-images.githubusercontent.com/103921593/229993174-5b67e57e-3e01-4ac4-9f83-410a932b22bf.png)

# Program :

```python

import numpy as np

# Number of arrivals (x)
x = np.array([0, 1, 2, 3, 4, 5])

# Frequency of arrivals (f)
f = np.array([5, 12, 18, 10, 3, 2])

# Total frequency
N = np.sum(f)

# Probability distribution P(x)
P = f / N

# Mean calculation
mean = np.sum(x * P)

# x^2 calculation
x2 = x ** 2

# E(x^2)
Ex2 = np.sum(x2 * P)

# Variance calculation
variance = Ex2 - (mean ** 2)

# Display results
print("Value of x :", x)
print("Frequency f :", f)
print("Probability P(x) :", P)

print("\nMean of the distribution =", round(mean, 4))
print("Variance of the distribution =", round(variance, 4))
```

# Output :
<img width="572" height="145" alt="image" src="https://github.com/user-attachments/assets/f58e2d34-0f66-47b7-9cc5-23234809f7ba" />


# Results :
The mean and variance of arrivals of objects from feeder using probability distribution are calculated.

