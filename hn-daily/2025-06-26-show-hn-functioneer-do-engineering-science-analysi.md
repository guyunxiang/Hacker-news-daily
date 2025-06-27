# Show HN: Functioneer – Do engineering/science analysis in under 5 lines of code

**Posted by qthedoc on 2025-06-26**

Hi HN, first post here!  
Functioneer is the ultimate batch runner. Prepare to become an analysis ninja. I hope to share it widely and get some feedback.

I've worked as a solar thermal engineer for years and was always surprised that there was no tool that made optimization and high-dimensional parameter testing straightforward. So, once I learned to code last year, I built one.

With Functioneer, every analysis is a series of steps where you can define parameters, create branches, execute or optimize functions, and save results as parameters. You can add as many steps as you like, applying them to all branches simultaneously. It’s very powerful!

### Example: Testing a Function Across a Parameter Grid

Here's how you can test any function across ranges of parameters (using the popular Rosenbrock function as an example):

```python
import functioneer as fn

# Insert your function here!
def rosenbrock(x, y, a, b):
    return (a - x) * 2 + (b - y) * 2

# Create analysis module with initial parameters
anal = fn.AnalysisModule({'a': 1, 'b': 100, 'x': 1, 'y': 1})

# Test over a grid of 'x' and 'y' values
anal.add.fork('x', (0, 1, 2))
anal.add.fork('y', (1, 10))
anal.add.execute(func=rosenbrock)

# Run the analysis and view results
print(anal.run()['df'][['x', 'y', 'rosenbrock']])
```

### Example Output:

| x | y | rosenbrock |
|---|---|------------|
| 0 | 1 | 101        |
| 0 | 10 | 10001     |
| 1 | 1 | 0          |
| 1 | 10 | 8100      |
| 2 | 1 | 901        |
| 2 | 10 | 3601      |

---

Feel free to ask questions or share feedback!