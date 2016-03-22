## ATIVIDADE-MAPA-ADIS-PROGRAMACAO-III

Construa uma classe Pessoa no arquivo classePessoa.php que estende a classe Banco (classeBanco.php) com os seguintes atributos:
* id (privado)
* cpf (público)
* nome (público)
* email (público)

Implemente os seguintes métodos:
* construtor
* getId 
* setId

Crie um arquivo chamado index.html que tenha um formulário que envie os dados para o arquivo cadastrarPessoa.php por método POST na seguinte configuração:
* Campo para o cpf
* Campo para o nome
* Campo para o email
* Botão de enviar o formulário

No arquivo cadastrarPessoa.php crie um objeto chamado pessoa que instancia a classe Pessoa, passados os dados de formulário como parâmetros para o construtor da classe. Execute o método salvar, que foi herdado na classe Pessoa pela classe Banco.

Crie uma variável que irá receber o retorno do método listar (herdado da classe Banco) do objeto pessoa e utilize as informações obtidas para montar uma tabela com os dados de todas as pessoas cadastradas (id, cpf, nome e email).

***Observação:***
* Não esqueça de criar uma tabela no banco de dados com o id como auto-incremento.
* Não esqueça de testar os parâmetros passados para o método construtor.
* A função mysql_fetch_object joga os valores do array no objeto antes de invocar o método construtor.
* O uso de uma folha de estilos para deixar a interface mais bonita é opcional.