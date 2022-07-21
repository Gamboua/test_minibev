# Mini BEV ~~(boolean é varchar)~~ Tests
## Por que testar?
Basicamente, testar código é rodar com um input controlado e checar o output esperado. Conforme o nosso código cresce, vai ser tornando uma tarefa difícil garantir, sempre que uma nova linha de código precisar ser acrescentada, que o código antigo não foi afetado.

Também, a medida que o código cresce, se torna cada vez mais difícil realizar os testes manualmente. Mesmo que tenhamos guardado tudo o que precisamos testar toda vez antes de subir um código para produção. 

Outra questão é que fazendo manualmente, estamos mais sussetível a erros humanos. O que torna a repetição dos testes algo não tão confiável.

Os testes ajudam a sabem se novos bugs não foram inseridos no código.
## Quais os tipos de test?
![Tipos de teste](/images/test_types.png)

### Unit tests
Consiste em testar individualmente as funções, métodos de classe, componentes ou módulos.
### Integration tests
Testes de integração garatem que os módulos ou serviços usados pela aplicação funcionam bem juntos. Por exemplo: testar interações com banco de dados ou chamada de alguma API.
### End-to-end tests
Testes end-to-end (e2e) reproduzem o comportamento do usuário em um ambiente completo. Verifica os vários fluxos e possibilidades que o usuário tem de navegação. Por exemplo: autenticar, carregar páginas com os componentes corretos, etc.
## O que testar?
Em nossas APIs costumamos testar:
- Helpers
- Serializers
- Views
- Métodos de classe
## Mocks
Mock é um processo usado nos testes unitários quando eles possuem dependencias externas. O proposito de mockar é focar no código sendo testado e não no comportamento ou estado da dependencias externa.
## Testes automatizados
Como os testes vão aumentando sempre, rodar eles individualmente se torna cada vez mais difícil. Por isso usamos ferramentas que conseguem repetir todos os testes sempre que precisamos com apenas um comando e no final, temos o relatório de quais testes falharam, por que e onde falharam.
## Bibliotecas de test
A biblioteca que usamos no backend para testar é o Pytest
## TDD
Test-Driven Development (TDD) é uma prática de programação que implica em escrever o teste antes de escrever o código que será executado. Esse processo força o programador a pensar antes na interface e nos resultados esperados.
TDD possui alguns passos:
- Escrever os testes que irão falhar (isso pq o código ainda nem foi escrito ainda)
- Escrever o código mínimo para que o teste passe 
- Refatorar o código e adicionar novos casos se for necessário
- Rodar os testes para ver se não quebraram 
- repetir

O objetivo é uma forma do programador escrever sempre melhores códigos de forma objetiva, simples e limpa.
## Referências
O que são testes de código
https://www.atlassian.com/continuous-delivery/software-testing/types-of-software-testing
https://blog.devgenius.io/what-is-testing-code-56b82d329fea

Difereças entre Testes unitários e Testes integrados
https://www.guru99.com/unit-test-vs-integration-test.html
https://www.guru99.com/integration-testing.html

Mocking
https://www.telerik.com/products/mocking/unit-testing.aspx#:~:text=Mocking%20is%20a%20process%20used,or%20state%20of%20external%20dependencies
https://stackoverflow.com/a/2666006

Livros
https://pragprog.com/titles/bopytest/python-testing-with-pytest/
https://www.estantevirtual.com.br/livrariaeconomica/kent-beck-tdd-desenvolvimento-guiado-por-testes-3269886444?show_suggestion=0
https://www.estantevirtual.com.br/livros/martin-fowler/refactoring-improving-the-design-of-existing-code/2695682573?show_suggestion=0&cep=8240005

/Users/gabriel/.ssh/test_minibev/README.md