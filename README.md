# Curso de Vue

- [Github do curso](https://github.com/matheusbattisti/curso_vue_yt)


## [Input e data binding](./exemplos_aula/2_input_e_data_binding/)
- Uma das funcionalidades mais interessantes é o **data binding**
- Onde temos a possibilidade de **mudar em tempo real um dado**, por meio do que é recebido de um input, por exemplo;
- O Vue torna isso mais fácil ainda, **algumas linhas e pronto**

- **v-model:** - 
- **v-on:click** - diretiva de click


## [O CLI do Vue](./exemplos_aula/3_projeto_cli/)
- O **CLI** é uma ferramenta de linha de comando do Vue
- Possibilita **criar e configurar** projetos de forma mais avançada
- **Por exemplo:** adicionar o Vue Router desde a instalação do projeto
- Isso flexibiliza muito as coisas


- npm i -g @vue/cli
- vue -V
- vue create 2_projeto_vue
- npm run serve


## [Componentes](./exemplos_aula/4_componentes/)
- É por meio de **Componentes** que podemos dividir o nosso layout em partes
- **Cada componente tem a sua responsabilidade**, por exemplo: um componente que é uma tabela e outro que é um rodapé
- Dividir as entidades desta maneira deixa o projeto com uma **separação de responsabilidades** maior
- Cada um tendo seu CSS e também os dados que manipula

- [Vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur)


## [Dados nos componentes](./exemplos_aula/5_dados_em_componentes/)
- Os componentes podem conter dados
- Podemos **inicializar já com algum valor** e também modificar durante a execução do programa
- Os dados ficam em uma função chamada **data**
- Esta função deve retornar os dados em **formato de objeto**
 

## [Life cycle Hooks](./exemplos_aula/6_lifecycle_hooks/)
- O **Life Cycle Hooks** são eventos que podem ser ativados em determinadas partes da execução do programa
- Exemplo: **created**
- Executa o código a partir do momento que o componente é criado
- Estes gatilhos são interessantes para alterar a aplicação em diversas etapas diferentes


## [Hierarquia de componentes](./exemplos_aula/7_hierarquia_de_componentes/)
- É comum **componentes terem outros componentes** que dependem deles
- Ou seja, criamos uma **árvore de componentes**
- Precisamos tomar cuidado para isso não virar uma **bagunça**
- Com essa divisão de componentes em subcomponentes, separamos mais ainda as responsabilidade de cada um dos componentes


## [Diretivas](./exemplos_aula/8_diretivas/)
- As **diretivas** em Vue são muitas
- Por exemplo: **v-if**
- Pode mudar a exibição de uma parte do layout, baseada em uma condição
- **As diretivas são essenciais** para uma aplicação dinâmica
- Podemos alterar a lógica pelos valores inseridos em **data**


## Atributos dinâmicos
### [Argumentos](./exemplos_aula/9_argumentos/) 
- Os **argumentos são valores dinâmicos** que podem ser inseridos em:
  - **Diretivas:** baseados nestes valores para executar um determinado comportamento
  - **Atributos:** mudar URL de links ou src de imagens
  - Essenciais para alterar a experiência do usuário no uso da aplicação

- **v-bind** - v-bind:href para linkar no href a variável meu_link
  - pode usar também :src, :href


## [Métodos](./exemplos_aula/10_metodos/)
- Os **métodos** do Vue são como **funções**
- Podemos **executá-los baseados em eventos** ou por alguma lógica da aplicação
- Eles ficam em um objeto chamado **methods**
- Onde criamos as funções que posteriormente serão executadas


## [CSS Scoped e CSS global](./exemplos_aula/11_scoped_styles/)
- O **CSS** no Vue pode ser dividido em duas categorias
- **Global:** onde definimos no App, por exemplo, e se aplica a todos os elementos
- **Scoped:** onde cada componente pode ter seu estilo, deixando mais fácil de personalizar os elementos
- Geralmente utilizamos o scoped para estilizar os componentes individualmente

- <style></style> - Global em qualquer arquivo da hierarquia
- <style scoped></style> - Scoped, mudança só no componente


## [Renderização de listas](./exemplos_aula/12_list_rendering/)
- As listas (**arrays**) serão renderizadas por **diretivas**
- Utilizaremos **v-for** para isso
- O dado pode vir de **data**, como um array
- E cada item pode ser impresso **junto do HTML**


## [Eventos](./exemplos_aula/13_eventos/)
- Os **eventos** são utilizados para complementar ações dos usuários com ativações de métodos
- Temos diverso tipos de eventos me Vue, como o click: **@click**
- Que podem ser **adicionados diretamente a elementos do HTML**
- O evento recebe um "parâmetro" que é o método que será executado


## [Múltiplos Eventos](./exemplos_aula/14_multiplos_eventos/)
- O Vue também permite a entrada de **múltiplos eventos** em um único evento
- A sintaxe permanece a mesma
- Porém vamos **separar os eventos por vírgula**
- Isso permite **executar dois ou mais métodos com um click**, por exemplo


## [Reutilização de componentes](./exemplos_aula/15_reutilizacao_de_componentes/)
- No Vue é comum a **reutilização de componentes**
- Cada componente será completamente **independente**
- Podendo **ativar seus métodos e mudar seus dados**, assim que necessário
- Para utilizar o recurso, basta invocar novamente o componente após a importação do mesmo


## [Utilizando props](./exemplos_aula/16_props/)
- **Os componentes do Vue podem receber dados**, e este recurso é chamado de **props**
- As props podem ser passadas por **valores do data**, como também podemos **inserir diretamente** eles
- **Precisamos declarar as propriedades recebidas pelos componentes**, em um array ou objeto chamados props


## [Emit](./exemplos_aula/17_emit/)
- Utilzando o **$emit** é possível ouvir um evento de um componente filho em um componente pai
- Com isso, **podemos ativar comportamentos (como métodos)** no componente pai
- **O evento deve ser registrado** no componente
- E é preciso definir o que será feito com a ativação do evento na chamada do componente


## [Projeto](./exemplos_aula/18_projeto/)
### Criando o projeto do curso
- vue create .
  - Marcar Router
  - Yes para history mode
- npm run serve


### Criando uma API com JSON server
- npm install json-server
- "backend": "json-server --watch db/db.json" - no package.json
  - npm run backend


### Implementando o Vue Router
- <router-view></router-view>
- [Router](./exemplos_aula/18_projeto/src/router/index.js)


### Finalizando header e footer
- **box-sizing: border-box** - altera a forma como o tamanho total de um elemento é calculado.
  - Facilita o controle do layout.
  - Evita “estourar” a largura do elemento com padding e bordas.
  - Muito comum em resets de CSS


