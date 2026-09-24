# Base de Conhecimento

## Dados Utilizados

Descreva se usou os arquivos da pasta `data`, por exemplo:

| Fonte | Utilização no Agente |
|--------|---------------------|
| Yahoo Finance | Coleta de dados financeiros e notícias |
| GDELT | Coleta de informações sobre ativos financeiros |


---

## Adaptações nos Dados

> Você modificou ou expandiu os dados mockados? Descreva aqui.

Não irei utilizar os dados fornecidos, mas sim adaptar o uso de bibliotecas para que o agente seja capaz de coletá-las.

---

## Estratégia de Integração

### Como os dados são carregados?
> Descreva como seu agente acessa a base de conhecimento.

O agente será integrado com ferramentas que permitam a execução de programas em python. Uma vez que isso é possível, será possível que o agente crie, execute e obtenha informações advindas das bases de dados Yahoo Finance e de notícias a partir do GDELT. Com isso o agente será capaz de trazer informações e executar pequenos códigos que tragam pequenas análises de código.

### Como os dados são usados no prompt?
> Os dados vão no system prompt? São consultados dinamicamente?

Os dados serão consultados e mantidos em uma pequena memória caso o tema seja o mesmo (para evitar novas requisições quando não é necessário). Uma vez com os dados, o LLM será capaz de trazer informações de sentimento do mercado ou informações importantes trazidas pela consulta. O modelo também será capaz de executar pequenos scripts que realizem cálculos com os dados utilizados e trazer pequenas informações/insights para o analista utilizando o agente.

---

## Exemplo de Contexto Montado

> Mostre um exemplo de como os dados são formatados para o agente.

```
Dados do Cliente:
- Nome: João Silva
- Perfil: Moderado
- Saldo disponível: R$ 5.000

Últimas transações:
- 01/11: Supermercado - R$ 450
- 03/11: Streaming - R$ 55
...
```
