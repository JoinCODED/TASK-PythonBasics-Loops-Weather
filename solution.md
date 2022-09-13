```python
def printer(elements):
    for element in elements:
        print(element)

def to_celsius(temperatures):
    return [(temp - 32) * 5 / 9 for temp in temperatures]

def hottest_days(temperatures, threshhold):
    return [temp for temp in temperatures if temp > threshhold]

def print_hottest_days(temperatures, threshhold):
    filtered = hottest_days(temperatures, threshhold)
    mapped = to_celsius(filtered)
    printer(mapped)
```
