# **Imersão Dados Alura 4º Edição**
Aula oferecida por Alura e Creditas
 Aula ministrada por Thiago Gonçalves, Vivian Yamassaki e Paulo Silveira

# O que aprendemos:
01 - Aplicar Python, Pandas e Colab em Data Science.
<br>02 - Descobrir como iniciar uma carreira na ciência de dados.</br>
03 - Construir análises de dados e tirar suas próprias conclusões.
<br>04 - Discutir boas práticas para transmissão transparente e clara de informação.</br>
05 - Entender e criar seu primeiro modelo de Machine Learning

## Nesta imersão dados iremos utilizar uma base de dados do kaggle com 10.000 imóveis de São Paulo para aplicar e aprender alguns conceitos utilizando a bibliotca Pandas do Python. Além de usar matplotlib e seaborn para criar gráficos, e fazer predições utilizando machine learning.

# Limpeza de dados
Logo que pegamos um banco de dados, não sabemos como ele vai estar. Por isso a primeira coisa que devemos fazer é realizar uma checagem e ver se precisamos realizar alguma reestruturação, edição ou corrigir alguns dados.
Apenas um exemplo, podemos observar que "Valor" apesar de ser um número, é tratado pelo nosso banco de dados como um "object", o que muitas vezes pode ser uma String, além de ter o cifrão ao lado o que atrapalharia na hora de realizar algum tipo de análise. O primeiro passo é transforma-lo em Float.

![](https://i.imgur.com/TSTDyKU.png)

O que notamos logo em seguida, é que na mesma coluna "Valor" temos alguns casos em que aparecem como aluguel e não um único valor. O que com certeza nos traria dificuldades na hora de traçar uma média ou realizar algum gráfico. Por isso decidimos transformar todos os valoras em Float e remover do nosso banco de dados os casos de aluguel ou qualquer outro valor que não seja o que queremos.

![](https://i.imgur.com/AI1gp8p.png)

# Análise Exploratória
A Análise exploratória de dados consiste em examinar e estudar o nosso conjunto de dados para termos uma ideia de padrões, anomalias e criarmos hipóteses baseadas na informação que podemos receber. Um metódo muito simples de começar uma análise exploratória é usar o comando describe() da biblioteca pandas.

![](https://i.imgur.com/utDKlWA.png)

A princípio já podemos notar algumas coisas que fogem do padrão e que pode causar problemas na hora de traçar uma média, como por exemplo um imóvel com 750.000m, 40 banheiros, 50 vagas e no valor de R$65.000.000. No gráfico abaixo podemos ver como esse outlier afeta a nossa análise.

![](https://i.imgur.com/jzO2rAC.png)

# Desafio aula 2:
- Preço do metro quadrado por bairro
- Montar um gráfico com a média dos bairros.

![](https://i.imgur.com/iGqqsVY.png)
