# Assignment

## Brief

Write the Python codes for the following questions.

## Instructions

Paste the answer as Python in the answer code section below each question.

### Question 1

Question: How do you create a 2x2 subplot grid in matplotlib and select the first subplot?

Answer:

```python
fig, axs = plt.subplots(2, 2)  # Creates 2x2 grid
axs[0, 0].plot([1, 2, 3], [2, 4, 6])  # Plotting simple line plot to display some output
plt.show()

```

### Question 2

Question: How to plot a line and set the color to red and style to dash in a matplotlib plot?

```python
x = [1, 2, 3, 4]
y = [1, 4, 9, 16]
```

Answer:

```python
x = [1, 2, 3, 4]
y = [1, 4, 9, 16]

plt.plot(x, y, color='red', linestyle='--')  # or shorter: plt.plot(x, y, 'r--')
plt.show()

```

### Question 3

Question: How to plot a histogram with 30 bins for `data` in matplotlib?

```python
data = np.random.randn(1000)
```

Answer:

```python
data = np.random.randn(1000)
plt.hist(data, bins=30)
plt.title('Histogram with 30 bins')
plt.show()

```

### Question 4

Question: How can you set the x-axis and y-axis labels in a matplotlib plot?

Answer:

```python
plt.plot([1, 2, 3, 4], [1, 4, 9, 16])
plt.xlabel('X-axis Label')  # Set x-axis label
plt.ylabel('Y-axis Label')  # Set y-axis label
plt.show()

```

### Question 5

Question: How do you create a bar plot in seaborn using the `tips` dataset to show the average tip amount per day?

```python
import seaborn as sns
tips = sns.load_dataset('tips')
```

Answer:

```python
# Load the tips dataset from seaborn online built-in example dataset and create a bar plot showing average tip by day
tips = sns.load_dataset('tips') # if loading from tips.csv in data folder, tips = pd.read_csv('../data/tips.csv')
sns.barplot( data=tips, x='day', y='tip')
plt.title('Average Tip Amount by Day')
plt.show()
```

### Question 6

Question: How to create a box plot for total_bill categorized by day in the `tips` dataset using seaborn?

Answer:

```python
sns.boxplot( data=tips, x='day', y='total_bill')
plt.title('Distribution of Total Bill by Day')
plt.show()

```

## Submission

- Submit the URL of the GitHub Repository that contains your work to NTU black board.
- Should you reference the work of your classmate(s) or online resources, give them credit by adding either the name of your classmate or URL.
