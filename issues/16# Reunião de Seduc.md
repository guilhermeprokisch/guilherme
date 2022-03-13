# [\#16 Issue](https://github.com/guilhermeprokisch/ideias/issues/16) `open`: Reunião de Seduc
**Labels**: `Movva`


#### <img src="https://avatars.githubusercontent.com/u/12011070?u=f18e95eceaa97f69b9d0c5a06270d7bdfbc44b5a&v=4" width="50">[guilhermeprokisch](https://github.com/guilhermeprokisch) opened issue at [2020-08-20 18:48](https://github.com/guilhermeprokisch/ideias/issues/16):

# Modelo de previsão da evasão da Seduc

## Dados 
  3 Grandes Grupos:
  ![image](https://user-images.githubusercontent.com/12011070/90808700-d31dd000-e2f6-11ea-82fa-8a185eb2496d.png)

Eles pegam fontes externas (Quais?). Depois passam por um classificador padrão. Um AutoML da Azure, hoje está em Python.

Interessante! Eles usam a probabilidade por aluno e dá pro aluno no inicio do aluno. Vai dando a probabilidade de cada aluno de evadir.

Questão:

![image](https://user-images.githubusercontent.com/12011070/90809107-60612480-e2f7-11ea-910f-9ecba4121a7e.png) a taxa de evasão de escola TX_EVASAO não está contaminando ou são os dados históricos?

Existem outro modelo DGREM. 
![image](https://user-images.githubusercontent.com/12011070/90809215-85ee2e00-e2f7-11ea-8e94-83f9a13dcdcf.png)

Me perdi... como eles fizerma esse DGREM?

A Seduc bateu esse antigo modelo.

![image](https://user-images.githubusercontent.com/12011070/90809389-c6e64280-e2f7-11ea-85ab-fbe7d743d89e.png)

Questão: Eles tem os dados históricos das escolas? Sim. Falado no final da reunião

Eles querem fazer um modelo causal. Presciptive model.

![image](https://user-images.githubusercontent.com/12011070/90809608-1d538100-e2f8-11ea-8e84-fe98006aff91.png)

Questão: daria para pedir essa variavel de taxa de risco? Sim, já pedimos.

@Paula_Miranda disse que pode ter uma relação entre a falta dados e a taxa de evasão.. Menos dados/Dados faltando => mais evasão

@Diogo Lopes. Comentou sobre sobre uma análise que relaciona a falta de dados do aluno/os quenao tem telefone/ taxa de risco e covid. Para questão será que os que tinham alto risco e poucos dados  evadiram na crise de covid?

Lembrar que o projeto é sobre o uso do App. Ver com alguem que app é esse?
 
[Centro de midia](https://centrodemidiasp.educacao.sp.gov.br/)

#### <img src="https://avatars.githubusercontent.com/in/77300?v=4" width="50">[cogitable](https://github.com/apps/cogitable) commented at [2020-08-20 18:48](https://github.com/guilhermeprokisch/ideias/issues/16#issuecomment-679108956):

Cited on [Seduc](17#issuecomment-679108949)  
 > Já tivemos a [Reunião de Seduc](16)


-------------------------------------------------------------------------------



[Export of Github issue for [guilhermeprokisch/ideias](https://github.com/guilhermeprokisch/ideias).]
