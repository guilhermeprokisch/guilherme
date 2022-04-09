[200](https://github.com/guilhermeprokisch/ideias/issues/200) 
###### 




 ######  Mention in [AlgoExpert #194](AlgoExpert-#194)  
 > nonConstructibleChange ts
[typescript](typescript) e [javascript](javascript) o sort padrão é gramatical. Por isso tem que se colocar o parametro

``` typescript
 array.sort((x,y) => x-y )
```

```typescript
export function nonConstructibleChange(coins: number[]) {
  coins.sort((x,y) => x-y)
	let currentChangeCreated = 0
	for (let i=0; i < coins.length; i++){
		if (coins[i] > currentChangeCreated + 1){
			return currentChangeCreated + 1
		} 
		currentChangeCreated += coins[i]
	}
	return currentChangeCreated + 1
}
```

-------------------------------------------------------------------------------

