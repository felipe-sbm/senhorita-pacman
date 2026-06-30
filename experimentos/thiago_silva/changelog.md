# Changelog Individual - Thiago Silva
## Projeto: Ms. Pac-Man com Aprendizado por Reforço

---

## 10/06/2026

### Atividades Realizadas

* Avaliação do modelo já pré-implementando

### Decisões Tomadas

* Teste do modelo apenas com 5 episódios para testar o treinamento.

### Problemas Encontrados

* Nenhum problema encontrado.

### Resultados Obtidos

* Ambiente inicial funcionando corretamente.
* Resultado pouco satisfatório tendo em vista a pouca quantidade de episódios.

### Próximos Passos

* Ajustes nos parâmetros para realizar o treinamento real.

---

## 12/06/2026

### Atividades Realizadas

* Avaliação do modelo já pré-implementando

### Decisões Tomadas

* Ajustes nos seguintes parâmetros:
- GAMMA = 0.99
- EPSILON = 1.0
- EPSILON_MIN = 0.1
- EPSILON_DECAY = 0.99 (Ajustado para 0.99, a intenção é que o modelo atinga a fase de não explorar mais a partir do episódio 230.
- BATCH_SIZE = 32
- EPISODES = 500 (Aumento na quantidade de episódios de 5 para 500)

### Problemas Encontrados

* Modelo sendo utilizado no Colab e tendo interrupções pela plataforma, o que compromente o treinamento.

### Resultados Obtidos

* Ambiente inicial funcionando corretamente.
* Resultado pouco satisfatório tendo em vista a pouca quantidade de episódios.

---

## 15/06/2026

### Atividades Realizadas

* Avaliação do modelo já em andamento.

### Decisões Tomadas

Modelo sendo testado pelo colab, com salvamento a cada 10 episódios.

### Problemas Encontrados

* Modelo sendo utilizado no Colab e tendo interrupções pela plataforma, o que compromente o treinamento;
* Teste do modelo de forma local, porém o tempo para treinar seria inviável, pois é mais lento.

### Resultados Obtidos

* Ambiente inicial funcionando corretamente.
* Treinamento de 130/500 episódios.

### Próximos Passos

* Continuação do treinamento.

 ---

## 16/06/2026

### Atividades Realizadas

* Avaliação do modelo já em andamento.

### Decisões Tomadas

Modelo sendo testado pelo colab, com salvamento a cada 10 episódios.

### Problemas Encontrados

* Recompensas variadas a cada episódio, ficando pouco clara a evoluação do modelo com base na plotagem do gráfico com base nas recompensas.

### Resultados Obtidos

* Ambiente inicial funcionando corretamente.
* Treinamento de 260/500 episódios.

### Próximos Passos

* Continuação do treinamento.

*  ---

## 22/06/2026

### Atividades Realizadas

* Avaliação do modelo já em andamento.

### Decisões Tomadas

Modelo sendo testado pelo colab, com salvamento a cada 10 episódios.

### Problemas Encontrados

* Recompensas variadas a cada episódio, ficando pouco clara a evolução do modelo com base na plotagem do gráfico com base nas recompensas.

### Resultados Obtidos

* Ambiente inicial funcionando corretamente.
* Treinamento de 400/500 episódios.
* Ao realizar o teste do modelo com essa quantidade de episódios treinados, o modelo simplesmente decorou o caminho e não conseguia variar. Optamos por não mais treinar esse modelo.

### Próximos Passos

* Treinamento de um novo modelo que apresentou melhor resultado.
* Implementação de um Double DQN.

* *  ---

## 30/06/2026

### Atividades Realizadas

* Avaliação do modelo já em andamento.

### Decisões Tomadas

EPISODE_START = 3000
EPISODES = 5000
BATCH_SIZE = 128
MEMORY_SIZE = 20000  # ajustado para uso do colab gratuito
GAMMA = 0.99
LEARNING_RATE = 0.0001

EPSILON = 0.15
EPSILON_MIN = 0.1 #Chegou no mínimo por volta do 4700
EPSILON_DECAY = 0.999

Modelo sendo testado pelo colab, com salvamento a cada 10 episódios.

### Problemas Encontrados

* Tempo de execução ainda é demorado devido a limitação do colab.

### Resultados Obtidos

* Ambiente inicial funcionando corretamente.
* Treinamento de 4500 episódios
* Modelo aprendeu mais variações de caminhos a serguir, inclusive com pontuações acima dos 1000 nos testes.
* Não ficava travado em alguma parede devido a regra de penalidade se ficar parado por 40 passos.
* Quando havia menos bolinhas no cenário, o modelo buscava outras rotas visando fazer mais pontos.
* Não tinha o senso de fugir dos fantasmas ainda

### Próximos Passos

* Mais tempo de treinamento.




