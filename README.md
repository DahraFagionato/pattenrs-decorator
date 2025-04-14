![decorator](https://github.com/user-attachments/assets/dce3aa53-2e24-4e5d-bc95-157b59afa7e5)


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

#### Decorator X Singleton
O padrão Decorator e o padrão Singleton atendem a necessidades diferentes no design de software. O Decorator é ideal para adicionar funcionalidades de forma flexível, enquanto o Singleton é útil para garantir que uma classe tenha apenas uma instância. 


#### Demonstração


##### Padrão Decorator em Java

Este projeto demonstra a implementação do padrão de projeto Decorator em Java, utilizando uma classe base para bebidas e decoradores para adicionar ingredientes como leite e chocolate.

##### Estrutura do Projeto

O projeto é composto pelas seguintes classes:

- **Beverage**: Classe abstrata que define a interface para as bebidas.
- **Coffee**: Classe concreta que representa uma bebida específica (café)..
- **Milk**: Decorador que adiciona leite à bebida.
- **Chocolate**: Decorador que adiciona chocolate à bebida.

##### Exemplo de Uso

No exemplo, começamos com um objeto `Coffee` e, em seguida, adicionamos `Milk` e `Chocolate`:

```java
public class Main {
    public static void main(String[] args) {
        Bebida bebida = new Cafe();
        System.out.println(bebida.getDescricao() + " $" + bebida.custo());

        bebida = new Leite(bebida);
        System.out.println(bebida.getDescricao() + " $" + bebida.custo());

        bebida = new Acucar(bebida);
        System.out.println(bebida.getDescricao() + " $" + bebida.custo());
    }
}

```

##### Integrantes: Dahra Fagionato, Emily Goulart, Maria Eduarda Berto, Nicole Santos, Pedro Lima
