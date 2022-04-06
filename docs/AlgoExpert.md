[194](https://github.com/guilhermeprokisch/ideias/issues/194) 
###### 

Two Number Sum

Solution Python:
```python
def twoNumberSum(array, targetSum):
	for i, n in enumerate(array):
		if (targetSum - n) in array[i+1:]:
			return [n, targetSum-n]
	return []
````



-------------------------------------------------------------------------------

