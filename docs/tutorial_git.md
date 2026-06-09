# Tutorial Básico de Git e GitHub

## Objetivo
Este tutorial explica como baixar o projeto, criar alterações e enviar as modificações para o GitHub.

# 1. Instalar o Git
Verifique se o Git está instalado:

```bash
git --version
```
Se aparecer uma versão, o Git já está instalado.

Exemplo:
```bash
git version 2.49.0
```

# 2. Clonar o Repositório
Abra o terminal e execute:

```bash
git clone URL_DO_REPOSITORIO
```
Exemplo:

```bash
git clone https://github.com/usuario/ms-pacman-rl.git
```
Entre na pasta:

```bash
cd ms-pacman-rl
```

# 3. Atualizar o Projeto
Antes de começar a trabalhar:

```bash
git pull origin main
```
Isso baixa as alterações mais recentes.

# 4. Criar uma Branch
Cada integrante deve trabalhar em sua própria branch.

Exemplo:

```bash
git checkout -b samuel
```
ou

```bash
git checkout -b joao
```
Verificar branch atual:

```bash
git branch
```
A branch atual aparecerá com um asterisco:

```text
* samuel
  main
```

# 5. Verificar Arquivos Modificados
Após alterar algum notebook:

```bash
git status
```
Exemplo:

```text
modified: notebooks/03_modelo_dqn.ipynb
```

# 6. Adicionar Arquivos ao Commit
Adicionar tudo:

```bash
git add .
```
Ou apenas um arquivo:

```bash
git add notebooks/03_modelo_dqn.ipynb
```

# 7. Criar um Commit
Criar um commit descrevendo a alteração:

```bash
git commit -m "Implementa arquitetura inicial da DQN"
```
Outros exemplos:

```bash
git commit -m "Adiciona replay buffer"

git commit -m "Corrige preprocessamento"

git commit -m "Adiciona gráficos de avaliação"
```

# 8. Enviar para o GitHub
Primeiro envio da branch:

```bash
git push -u origin samuel
```

Próximos envios:

```bash
git push
```

# 9. Atualizar a Branch com Alterações da Main
Caso a branch principal seja atualizada:

```bash
git checkout main

git pull origin main

git checkout samuel

git merge main
```

# 10. Fluxo Completo
Sempre seguir esta sequência:

```bash
git pull origin main

# Fazer alterações

git add .

git commit -m "Descrição da alteração"

git push
```

# Boas Práticas
## Faça commits pequenos
Bom:

```bash
git commit -m "Implementa replay buffer"
```
Ruim:

```bash
git commit -m "Muitas coisas"
```

## Atualize seu changelog
Após concluir uma tarefa:

* Atualize seu arquivo de changelog.
* Descreva o que foi feito.
* Registre problemas encontrados.
* Registre resultados obtidos.

## Não editar a branch main diretamente
Todo desenvolvimento deve ocorrer em branches individuais.

# Em Caso de Problemas
Verificar branch atual:

```bash
git branch
```
Verificar arquivos modificados:

```bash
git status
```
Ver histórico de commits:

```bash
git log --oneline
```
Verificar repositório remoto:

```bash
git remote -v
```