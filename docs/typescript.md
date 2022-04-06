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

-------------------------------------------------------------------------------
