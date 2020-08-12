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
## ATENÇÃO PARA AS LETRAS MAIÚSCULAS E MINÚSCULAS. NO PYTHON ELAS FAZEM PARTE DA IDENTIDADE DO CÓDIGO E SEGUEM O PADRÃO DA LINGUAGEM!
~~~~python
from folium.plugins import HeatMap 
#Para executar o comando clique no Play ou use o atalho do teclado Shift+Enter
~~~~
