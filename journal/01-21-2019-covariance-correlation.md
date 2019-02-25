Description: A summary of covariance and correlation

References: 
  - [1] [Correlation and dependence](https://en.wikipedia.org/wiki/Correlation_and_dependence) 
  - [2] [What Is Correlation?](https://www.youtube.com/watch?v=Ypgo4qUBt5o)
  - [3] [Understanding Covariance](https://www.youtube.com/watch?v=xGbpuFNR1ME&list=PLIeGtxpvyG-JMH5fGDWhtniyET88Mexcw&index=6) 
  - [4] [The Covariance Matrix](https://www.youtube.com/watch?v=locZabK4Als&list=PLIeGtxpvyG-JMH5fGDWhtniyET88Mexcw&index=7)
  - [5] [Understanding Correlation](https://www.youtube.com/watch?v=4EXNedimDMs&list=PLIeGtxpvyG-JMH5fGDWhtniyET88Mexcw&index=8) 

### Covariance [3]
- bivariate relationships: relationships that involve aspects of two variables
- covariance is a descriptive measure of linear association between two variables
  - essentially, it asks 'how do two variables behave as a pair?'
- the sign of the covariant indicates if the relationship is increasing/decreasing
  - if variables move in the same direction, then the covariance is positive, otherwise it's negative 
- only interested in the sign/direction, not the strength of the direction (unless it's close to `0`)
  - if the two variables don't exhibit any kind of pattern, then the covariance will be close to `0`
  - the covariance doesn't say anything about the strength of the linear relation

### Covariance Matrix [4]
- a covariance matrix simply computes the covariance between each variable pair
- the diagonal of a covariance matrix provides the variance of each individual variable (covariance with itself)
  - notice the standard deviation is just the square root of the variance (so it can also be computed from the covariance matrix)

### Correlation
- a covariance provides the direction of the linear relationship between two variables, while correlation provides direction and strength [5]
- a covariance has no upper/lower bounds (its size is dependent on the scale of the variables), correlation is always in `[-1,1]` (its scale is independent of the scale of the variables themselves) [5]
  - i.e., covariance is not standardized, while correlation is 
- a correlation is the linear relationship between two variables [2]
  - it's only applicable to linear relationships [5]
- [formula (and equivalent expressions)](https://en.wikipedia.org/wiki/Pearson_correlation_coefficient#For_a_sample)
- correlation might be indicative of a predictive relationship [1]
- the presence of a correlation is not enough to infer a causal relationship (i.e., correlation does not imply causation) [1]
- direction of the correlation [2]
  - `r=[0, 1]`: a positive correlation occurs when both variables are increasing/decreasing at the same time (i.e., as the variable `x` increases, so does `y`)
  - `r=[0, -1]`: a negative correlation exists when the variables are going in opposite directions
  - the data might have no correlation at all
- strength of correlation [2]
  - the closer `r` is to `1` (regardless of its sign), the stronger the correlation is
