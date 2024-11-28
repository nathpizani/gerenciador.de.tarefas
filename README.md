# gerenciador.de.tarefas
# Gerenciador de Tarefas

## Objetivo
Desenvolver um script simples para gerenciar tarefas, permitindo adicionar, listar e remover tarefas.

## Funcionalidades
1. Adicionar uma nova tarefa.
2. Listar todas as tarefas pendentes.
3. Remover tarefas concluídas.

## Cronograma
-  Configuração do repositório e README.md: **1º dia**
-  Implementação da funcionalidade de adicionar tarefas: **2º dia**
-  Implementação da funcionalidade de listar tarefas: **3º dia**
-  Implementação da funcionalidade de remover tarefas: **4º dia**
-  Testes e documentação final: **5º dia**



##CÓDIGO DESENVOLVIDO:
tarefas = []

def adicionar_tarefa(tarefa):
    tarefas.append(tarefa)
    print(f"Tarefa '{tarefa}' adicionada com sucesso!")

def listar_tarefas():
    if not tarefas:
        print("Nenhuma tarefa pendente.")
    else:
        print("Tarefas pendentes:")
        for i, tarefa in enumerate(tarefas, start=1):
            print(f"{i}. {tarefa}")

def remover_tarefa(indice):
    try:
        tarefa_removida = tarefas.pop(indice - 1)
        print(f"Tarefa '{tarefa_removida}' removida com sucesso!")
    except IndexError:
        print("Índice inválido!")

# Menu interativo
tarefas = []

def adicionar_tarefa(tarefa):
    tarefas.append(tarefa)
    print(f"Tarefa '{tarefa}' adicionada com sucesso!")

def listar_tarefas():
    if not tarefas:
        print("Nenhuma tarefa pendente.")
    else:
        print("Tarefas pendentes:")
        for i, tarefa in enumerate(tarefas, start=1):
            print(f"{i}. {tarefa}")

def remover_tarefa(indice):
    try:
        tarefa_removida = tarefas.pop(indice - 1)
        print(f"Tarefa '{tarefa_removida}' removida com sucesso!")
    except IndexError:
        print("Índice inválido!")

