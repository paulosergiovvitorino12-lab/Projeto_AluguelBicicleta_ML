# Situação-problema: quanto custa alugar uma bicicleta?

## Contexto

A Pedal Livre é uma pequena loja de aluguel de bicicletas localizada perto de um parque. Antes de iniciar o passeio, os clientes costumam perguntar quanto pagarão pelo tempo que pretendem ficar com a bicicleta.

A loja possui registros de aluguéis anteriores, mas precisa de uma maneira simples de estimar o preço para diferentes durações. Os valores históricos apresentam pequenas variações devido a descontos aplicados em alguns atendimentos.

Você foi contratado como **analista de dados** para desenvolver uma solução que utilize esses registros para prever o preço de um aluguel a partir da duração do passeio.

## Dados históricos

Todos os registros representam o aluguel do mesmo tipo de bicicleta. Os dados são fictícios e foram preparados para esta atividade.

| Duração do aluguel (minutos) | Preço pago (R$) |
|---:|---:|
| 10 | 10,00 |
| 15 | 13,00 |
| 20 | 14,00 |
| 25 | 18,00 |
| 30 | 19,00 |
| 35 | 23,00 |
| 40 | 24,00 |
| 50 | 30,00 |
| 55 | 32,00 |
| 60 | 34,00 |

## Sua missão

A gerente precisa responder à seguinte pergunta:

> Qual é o preço estimado para um cliente que deseja alugar uma bicicleta por 45 minutos?

Desenvolva uma solução em um Jupyter Notebook, utilizando Python e o modelo **LinearRegression do Scikit-learn**. Use somente uma variável de entrada: a duração do aluguel em minutos. O valor que deverá ser previsto é o preço em reais.

## Roteiro de trabalho

1. **Compreenda os dados.** Observe a tabela e descreva o que geralmente acontece com o preço quando a duração do aluguel aumenta.
2. **Organize os registros.** Represente os dados usando listas Python. Mantenha cada duração associada ao preço correspondente. Organize as entradas como uma tabela de uma coluna, com uma lista interna para cada aluguel.
3. **Prepare o modelo.** Importe o LinearRegression e crie um modelo de regressão linear.
4. **Treine o modelo.** Utilize as durações e os respectivos preços históricos para que ele aprenda a relação entre essas informações.
5. **Faça a previsão principal.** Solicite ao modelo uma estimativa para um aluguel de 45 minutos.
6. **Explore outras durações.** Faça também previsões para aluguéis de 20 e 60 minutos. Compare os resultados com os preços registrados na tabela. Eles precisam ser exatamente iguais? Explique sua resposta.
7. **Comunique sua conclusão.** Escreva uma resposta curta para a gerente, informando o preço estimado para 45 minutos e explicando como você chegou a esse resultado.

## Perguntas para a análise

- Qual é a variável de entrada e qual é a variável que queremos prever?
- Qual preço o modelo estimou para 45 minutos?
- As previsões para 20 e 60 minutos ficaram próximas dos valores históricos?
- Por que o preço previsto deve ser apresentado como uma estimativa?
- Você teria a mesma confiança em uma previsão para 300 minutos? Justifique considerando os dados disponíveis.

## Orientações

- Utilize apenas listas Python e Scikit-learn. Não é necessário usar Pandas, importar NumPy ou criar gráficos.
- Preserve a ordem dos registros: cada duração deve corresponder ao preço na mesma posição.
- Apresente os preços em reais, com duas casas decimais.
- A regressão busca uma tendência geral: ela não precisa reproduzir exatamente cada preço histórico.
- A comparação com preços usados no treinamento ajuda a observar o ajuste, mas não comprova que o modelo terá bom desempenho em novos aluguéis. Nesta atividade introdutória, o objetivo é praticar o treinamento e a previsão.

## Entrega

Entregue um Jupyter Notebook contendo seu nome, os dados organizados, o treinamento do modelo, as três previsões solicitadas e as respostas às perguntas de análise.

Finalize com um pequeno parecer para a gerente da Pedal Livre. Use uma linguagem simples, como um analista de dados explicando seu resultado a alguém que não conhece programação.
