<img src="imagens/decorator.jpg" alt="Descrição da imagem" width="300"/>

#### Definição
O padrão Decorator permite adicionar responsabilidades a um objeto de forma dinâmica. É uma alternativa flexível à subclasse para estender funcionalidades.

#### Porque o Decorator?
- É visual, fácil de demonstrar com exemplos reais (tipo montar um café com extras).
- Permite adicionar funcionalidades dinamicamente sem alterar a estrutura original do objeto.
- Muito usado em frameworks de UI, streams de dados, filtros, etc.

#### Vantagens
- Flexível: adiciona comportamentos sem mexer no código original.
- Evita explosão de subclasses.
- Pode combinar múltiplos comportamentos em tempo de execução.

#### Desvantagens
- Pode introduzir muitos objetos pequenos, dificultando o debug.
- A estrutura encadeada pode ser difícil de entender se muito complexa.
- Nem sempre é óbvio quem está decorando quem.
