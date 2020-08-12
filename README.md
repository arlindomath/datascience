# Data Science

## Mapas 

Os mapas são instrumentos de comunicação, são utilizados para representar graficamente área do espaço terrestre. Através de diferentes tipos de informações é possível construir diversos tipos de mapas.

![Mapa Mundi](https://images.unsplash.com/photo-1526667383715-3c42cbae3d60?ixlib=rb-1.2.1&q=85&fm=jpg&crop=entropy&cs=srgb&ixid=eyJhcHBfaWQiOjYzOTIxfQ)


### Mapa de calor


O mapa de calor mostra quais são os pontos quentes dos dados. Com ele podemos identificar as regiões com maior concentração de casos de Covid-19. Para construir esse Mapa utilizaremos a Biblioteca Folium - Acesse a documentação: https://python-visualization.github.io/folium/

## VAMOS AO CÓDIGO!

Para instalar o Folium no [Colab Notebook](https://colab.research.google.com/) utilizamos o pip. O pip é o instalador de pacotes do Python, linguagem que estamos utilizando:
~~~python
!pip install folium 
#Para executar o comando clique no Play ou use o atalho do teclado Shift+Enter
~~~~
Depois de instalar a biblioteca, devemos importá-la para o nosso código:
~~~python
import folium 
#Para executar o comando clique no Play ou use o atalho do teclado Shift+Enter
~~~~
Com o folium presente, temos então a facilidade de importar o modelo de Mapa de Calor presente nos *plugins* da biblioteca, aqui então importaremos o HeatMap:
###### ATENÇÃO PARA AS LETRAS MAIÚSCULAS E MINÚSCULAS. NO PYTHON ELAS FAZEM PARTE DA IDENTIDADE DO CÓDIGO E SEGUEM O PADRÃO DA LINGUAGEM!
~~~~python
from folium.plugins import HeatMap 
#Para executar o comando clique no Play ou use o atalho do teclado Shift+Enter
~~~~
Ao concluir todas as importações referentes ao Folium, partimos para a famigerada biblioteca Pandas, importantíssima para o nosso trabalho com dados. Com ela podemos além de importar dados também podemos editá-los:
#### Pandas é o nome da biblioteca e como de costume os programadores as apelidam de pd, mas isso é opcional.
```python
import pandas as pd 
#Para executar o comando clique no Play ou use o atalho do teclado Shift+Enter
```
Agora de fato iremos trabalhar com os nossos dados! Em Python assim como em outras linguagens precisamos nos atentar para algumas informações, como por exemplo o sinal de igual (=). Aqui esse sinal quer dizer que alguma variável **RECEBE** informações de um DataFrame (Matriz de Dados), perceba que eu enfatizei a palavra recebe, isso porque no Python o sinal de igual isolado quer dizer exatamente isso. Se eu quiser usar o sinal de igual aqui eu utilizo dois sinais (==), por exemplo 1 == 1.

Seguindo com o código, a variável (dados_covid19) irá receber informações de um arquivo csv.

Nesse caso utilizarei os arquivos disponibilizados no [Github do Wesley Cota](https://github.com/wcota/covid19br):
```python
dados_covid19 = pd.read_csv('https://raw.githubusercontent.com/wcota/covid19br/master/cases-gps.csv') 
#Para executar o comando clique no Play ou use o atalho do teclado Shift+Enter
```

