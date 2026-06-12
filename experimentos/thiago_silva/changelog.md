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

### Próximos Passos

* Implementação de salvamento automático a cada x quantidade episódios treinados.



