# Fórum de Comentários em Árvore

Projeto desenvolvido para a disciplina de Estrutura de Dados.

## Descrição

O sistema simula um fórum de discussões utilizando uma estrutura de árvore. Cada comentário pode possuir respostas, formando uma hierarquia de comentários e subcomentários.

A raiz da árvore é um nó especial chamado **DISCUSSÃO**, responsável por agrupar todos os comentários principais.

Exemplo:

```text
DISCUSSÃO
├── Comentário 1
│   ├── Resposta 2
│   └── Resposta 3
└── Comentário 4
```

## Funcionalidades

* Criar comentários
* Responder comentários
* Editar comentários
* Remover comentários e suas subárvores
* Navegar entre comentários
* Exibir caminho até um comentário
* Exibir a árvore completa
* Listar comentários folha
* Contabilizar comentários

## Estrutura do Projeto

```text
Comentario.java
ComentarioTree.java
ForumService.java
UI.java
Main.java
```

### Comentario

Representa um nó da árvore.

### ComentarioTree

Responsável pelas operações sobre a árvore de comentários.

### ForumService

Contém a lógica de negócio e interação com o usuário.

### UI

Responsável pela exibição das informações.

### Main

Ponto de entrada da aplicação.

## Comandos

| Comando | Descrição |
|----------|------------|
| C | Criar um novo comentário ou resposta ao comentário atual |
| E | Editar o comentário atual |
| D | Excluir o comentário atual |
| V | Navegar para um comentário informando seu ID |
| B | Retornar ao comentário pai |
| B0 | Retornar à conversa principal |
| F | Listar todos os comentários folha da árvore |
| A | Exibir a estrutura completa da árvore de comentários |
| U | Exibir todos os comentários de um autor |
| M | Exibir o menu de comandos |
| S | Encerrar o sistema |


## Equipe e Divisão de Responsabilidades

| Integrante                                | GitHub                      | Responsabilidades                                                                                                                                                                                                                                               |
| ----------------------------------------- | --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Ana Clara Marinho Viana                   | @anaclaramarinhoviana77-alt | Implementação dos métodos de percurso da árvore, com foco na geração da representação textual completa da estrutura de comentários (`gerarArvoreTexto`).                                                                                                        |
| Charles Brendon Silva Suzart              | @CharlesBrendonIF           | Desenvolvimento da classe `Comentario`, incluindo finalização da modelagem da entidade, getters, setters e revisão geral da classe.                                                                                                                             |
| Emanuel Fonseca Nogueira                  | @Nuillexe                   | Scrum Master e Gerente de Projeto. Responsável pelo planejamento do projeto, organização do repositório, criação de branches, revisão de Pull Requests, resolução de conflitos, implementação da classe `Main`, testes finais e integração de todos os módulos. |
| Indaiá                                    |                             | Implementação dos métodos de folhas e estatísticas da árvore, incluindo `listarFolhas()` e `contarComentarios()`.                                                                                                                                               |
| Kaique Santos Moreira                     | @KaiqueFullDev              | Implementação da interface textual (`UI`), incluindo exibição de comentários, menus, folhas, árvore de comentários e demais funcionalidades de interação com o usuário.                                                                                         |
| Maria Eduarda De Oliveira Ferreira Santos | @eduardasxntos              | Implementação da classe `ComentarioTree`, com foco nos métodos de remoção de comentários, obtenção do caminho de navegação e seleção (`removerComentario()`, `obterCaminho()` e `comentariosDoAutor`).                                                                                         |
| Pedro                                     |                             | Implementação da classe `ForumService`, incluindo criação, edição e remoção de comentários, navegação entre comentários e leitura de comandos do usuário.                                                                                                       |

</table>






  
