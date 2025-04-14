<![decorator](https://github.com/user-attachments/assets/eacf9d77-f4c3-49c9-9568-cfa0de3452a7) widht="300">

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
