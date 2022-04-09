[195](https://github.com/guilhermeprokisch/ideias/issues/195) 
###### 

Tails no Typescript são os slice simples ex: arr.slice(2)


Site interessante https://wanago.io/2019/03/25/node-js-typescript-7-creating-a-server-and-receiving-requests/ para fazer um servidor http com node puro e Typescript


Errei na solução em typescript do [AlgoExpert](AlgoExpert) pois pensei que o 'in' do Js era similar ao do Python. Não, o in do JS é para verificar se uma propriedade está em um objeto. E não para ver se algum elemento está em um array


https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Operators/in


 ######  Mention in [AlgoExpert #194](AlgoExpert-#194)  
 > Solução em [typescript](typescript)

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


<img width="1225" alt="image" src="https://user-images.githubusercontent.com/12011070/162054739-baf969c3-d04a-41d1-9c78-d87109467fe2.png">


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

