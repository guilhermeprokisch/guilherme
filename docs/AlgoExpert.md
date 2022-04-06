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


 ######  Mention in [typescript #195](typescript-#195)  
 > Errei na solução em typescript do [AlgoExpert](AlgoExpert) pois pensei que o 'in' do Js era similar ao do Python. Não, o in do JS é para verificar se uma propriedade está em um objeto. E não para ver se algum elemento está em um array


Solução em [typescript](typescript)

```typescript
export function twoNumberSum(array: number[], targetSum: number) {
	
	for(let i=0; i < array.length; i++){
		if( array.slice(i+1).include(targetSum - array[i]) ){
			return [array[i], targetSum - array[i]]
		}
	}
  return [];

}
```

-------------------------------------------------------------------------------
