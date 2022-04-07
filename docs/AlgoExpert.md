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


Validate subsequence:

```python
def isValidSubsequence(array, sequence):
    if array == [] and sequence != []:
        return False

    if sequence == []:
        return True

    head_array = array[0]
    head_sequence = sequence[0]
    tail_array = array[1:]
    tail_sequence = sequence[1:]

    if head_array == head_sequence:
        return isValidSubsequence(tail_array, tail_sequence)    
    return isValidSubsequence(tail_array, sequence)
```


Solução em TS

```typescript

export function isValidSubsequence(array: number[], sequence: number[]): boolean {
	if (array.length == 0 && sequence.length > 0){
			return false
	}
		
	if (sequence.length == 0){
		return true
	}
			
	let headSequence:number = sequence[0]
	let tailSequence:number[] = sequence.slice(1)
	
	let headArray:number = array[0]
	let tailArray:number[] =  array.slice(1)
	
	if (headArray == headSequence){
		return isValidSubsequence(tailArray, tailSequence)
	}
	return isValidSubsequence(tailArray, sequence)
	
}



```

-------------------------------------------------------------------------------

