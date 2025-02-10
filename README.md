
**Explicação do Código**

input("Qual a sua idade? ")
O input() exibe uma mensagem e espera que o usuário digite um valor.
Por padrão, input() retorna uma string, então precisamos converter para número.
int(input(...))
Como a idade é um número inteiro, usamos int() para converter a entrada.
Se o usuário digitar um valor decimal (ex: 25.5), o código dará erro. Para evitar isso, poderíamos usar float().
print(f"A idade do usuário é {idadeUser} anos.")
Aqui usamos f-strings (format strings) para inserir o valor dentro da mensagem.
O f antes das aspas permite incluir variáveis dentro das {} de forma clara e legível.
Possíveis Melhorias
Se quisermos evitar erros caso o usuário digite um valor inválido, podemos tratar exceções:

    try:
        idadeUser = int(input("Qual a sua idade? "))
        print(f"A idade do usuário é {idadeUser} anos.")
    except ValueError:
        print("Por favor, digite um número inteiro válido.")

Agora, se o usuário digitar "vinte" ao invés de 20, o programa exibe uma mensagem amigável em vez de gerar um erro.
## **Conclusão**

Esse pequeno exercício ensina conceitos fundamentais da programação em Python, como:  
✅ **Entrada de dados** com `input()`  
✅ **Conversão de tipos** com `int()`  
✅ **Manipulação de strings** com f-strings  
✅ **Tratamento de erros** para evitar que o programa quebre
