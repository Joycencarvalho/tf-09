# TF 09 - O Atalho na árvore

- **Encapsulamento:** a interface é a property `destino` (só leitura) e o método `redirecionar()`; a implementação é o atributo privado `__destino` e a validação que impede ciclos.
- **Herança:** a interface é tudo que o Atalho herda de Item (`nome`, `pai`, `caminho()`, `mover_para()`); a implementação fica no Item, e o Atalho só acrescenta o destino.
- **Polimorfismo:** a interface é a chamada `tamanho()` e `mostrar()`, igual para qualquer item; a implementação é o jeito do Atalho responder: 1 byte e `nome -> caminho do destino`.
- **Interface (Medivel):** o `espaco_total()` só precisa saber que existe `tamanho()`; ele não sabe que está somando um Atalho.