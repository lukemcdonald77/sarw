```python
position_visits,simulations, size = saw(100, 100)
visits_2d = [[0 for _ in range(size)] for _ in range(size)]
for (x, y), visits in position_visits.items():
    visits_2d[x][y] = visits
visits_array = np.array(visits_2d)

sns.heatmap(visits_array)
```

    Failures: 100 | Total Steps: 6950 | Average Steps: 69.5
    
![png](output_1_2.png)
    
```python
