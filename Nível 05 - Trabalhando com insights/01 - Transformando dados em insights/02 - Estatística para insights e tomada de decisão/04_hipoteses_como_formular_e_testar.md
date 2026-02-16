# Hipóteses: como formular e testar

## Por que aprender sobre Hipóteses?

Toda tomada de decisão baseada em dados começa com uma pergunta. E essa pergunta vira uma hipótese.

## O que é uma Hipótese?

Uma hipótese é uma afirmação testável sobre uma população.

Exemplo: "A campanha A gera mais cliques que a campanha B"

Importante: toda hipótese precisa ser clara, objetiva e mensurável.

## Hipótese Nula (H0) e Alternativa (H1)

- ➔ H0 (nula): é a afirmação de que não existe efeito, diferença ou relação.
- ➔ H1 (alternativa): é a afirmação que queremos testar, indicando a existência de um efeito, diferença ou relação.

Exemplo:

- ● H0: A campanha A tem a mesma taxa de cliques que a campanha B.
- ● H1: A campanha A tem uma taxa de cliques diferente da campanha B.

## Diferença de H0 para H1

Imagine que H₀ é a "presunção de inocência". Você só pode rejeitá-la se tiver evidências suficientes.

- ➔ H₀: “A pessoa é inocente.”
- ➔ H₁: “A pessoa é culpada.”

Você só rejeita H₀ (inocente) se os dados (as provas) forem fortes o suficiente.

![H0 x H1](assets/attachment_21.png)

## Como aparece na prática?

Você quer saber se uma nova política de desconto aumentou o ticket médio de compras no seu e-commerce.

- H₀: O ticket médio não mudou (foi igual ao antes da política).
- H₁: O ticket médio mudou.

Aprofundamento: Se você usar um teste t e encontrar um valor-p < 0.05, você pode dizer que há evidência suficiente para rejeitar H₀. Isso não garante que H₁ é verdadeira, mas indica que a mudança observada não parece ser fruto do acaso.

### ❗ IMPORTANTE❗

Você nunca “prova” H₀ ou H₁. Você rejeita ou não rejeita H₀.
Se não houver evidência, você não rejeita H₀. Mas isso não quer dizer que H₀ é verdadeira. Talvez você só precise de mais dados.

## Por que isso importa?

Um e-commerce quer testar se um cupom de desconto de R$ 20 está aumentando o número de vendas. O time de dados foi acionado para responder à pergunta:

“O cupom de R$ 20 está funcionando?”

Hipótese mal formulada (comum em iniciantes):

- ➔ H₀: O cupom de R$ 20 aumenta as vendas
- ➔ H₁: O cupom de R$ 20 não aumenta as vendas

🛑 Erro aqui:

A hipótese nula deve representar o estado padrão, ou seja, que não há diferença.
Se você coloca o efeito esperado como H₀, está invertendo a lógica do teste estatístico.

## Como Formular uma Hipótese

PASSO-A-PASSO

1. Parta de uma pergunta de negócio clara
2. Identifique as variáveis envolvidas
3. Defina H0 e H1 de forma mensurável

Exemplo:

- ➔ Pergunta: "Clientes com plano premium compram mais?"
- ➔ H0: Não há diferença no valor de compra entre planos.
- ➔ H1: O plano premium tem maior valor de compra médio.

### Exemplo 1 – Marketing

- ➔ A nova campanha aumentou as vendas?
- ➔ H₀: A média de vendas com a nova campanha é igual à da anterior.
- ➔ H₁: A média de vendas com a nova campanha é maior que a da anterior.

### Exemplo 2 – RH

- ➔ Funcionários com mais tempo de casa estão mais satisfeitos?
- ➔ H₀: O tempo de casa não influencia o nível de satisfação.
- ➔ H₁: Quanto maior o tempo de casa, maior a satisfação.

### Exemplo 3 – Produto

- ➔ A mudança no app reduziu o tempo de carregamento?
- ➔ H₀: O tempo de carregamento é o mesmo após a mudança.
- ➔ H₁: O tempo de carregamento é menor após a mudança.

## Tipos de Hipóteses

### Unicaudal: quando o interesse é saber se um grupo é maior ou menor.

- ➔ Pergunta: “A nova campanha aumentou as vendas?”
- ➔ H₀: A média de vendas nova é menor ou igual à antiga.
- ➔ H₁: A média de vendas nova é maior.

### Bicaudal: quando só queremos saber se é diferente

- ➔ Pergunta: “Será que a nova embalagem afeta a média de vendas?”
- ➔ H₀: A média de vendas é igual antes e depois da mudança.
- ➔ H₁: A média de vendas é diferente (pode ser maior ou menor).

## Aplicando em Testes

A hipótese define qual teste estatístico será aplicado:

- ➔ Diferença de médias? Teste t.
- ➔ Três ou mais grupos? ANOVA.
- ➔ Proporções? Teste qui-quadrado.

## Cuidados ao Formular

- ➔ Hipóteses muito genéricas ou subjetivas
- ➔ Falta de definição de métrica clara
- ➔ Comparar grupos com tamanhos muito diferentes
- ➔ Testar muitas hipóteses ao mesmo tempo (inflaciona chance de erro)

## Atividade prática

### Pergunta A:

A nova página de produto aumentou a taxa de cliques?

Resposta:

- ➔ H₀: A nova página tem a mesma taxa de cliques que a anterior.
- ➔ H₁: A nova página tem uma taxa de cliques maior do que a anterior.
- ➔ Tipo de hipótese: Unicaudal (direção esperada é "maior").

### Pergunta B:

Existe alguma diferença no ticket médio entre clientes do Plano A e do Plano B?

Resposta:

- ➔ H₀: O ticket médio dos clientes dos planos A e B é igual.
- ➔ H₁: O ticket médio dos clientes dos planos A e B é diferente.
- ➔ Tipo de hipótese: Bicaudal (a direção não é definida previamente).

### Pergunta C:

Depois do treinamento, os funcionários estão menos tempo ociosos?

Resposta:

- ➔ H₀: O tempo médio de ociosidade não diminuiu após o treinamento.
- ➔ H₁: O tempo médio de ociosidade diminuiu após o treinamento.
- ➔ Tipo de hipótese: Unicaudal (espera-se uma redução).

## Conclusão

Formular bem uma hipótese evita erros e economiza tempo…
