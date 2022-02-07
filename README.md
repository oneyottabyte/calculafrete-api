# API REST - CalculaFrete (Projeto Backend)


<h1 id="objetivo">
	<img src="https://img.icons8.com/external-tal-revivo-color-tal-revivo/24/000000/external-readme-is-a-easy-to-build-a-developer-hub-that-adapts-to-the-user-logo-color-tal-revivo.png"/>
  Objetivo do Projeto
</h1>

Implementar para empresa de transporte de cargas SigaBem o endpoint para o cálculo do preço do frete:

Você deve calcular o valor total do frete e a data prevista da entrega.

Considerar regras para calcular o valor do frete:
 * CEPs com DDDs iguais tem 50% de desconto no valor do frete e entrega prevista de 1 dia
 * CEPs de estados iguais tem 75% de desconto no valor do frete e entrega prevista de 3 dias
 * CEPs de estados diferentes não deve ser aplicado o desconto no valor do frete e entrega prevista de 10 dias
 * O valor do frete é cobrado pelo peso da encomenda, o valor para cada KG é R$1,00

Seu input de entrada deve ser “peso”, “cepOrigem”, “cepDestino” e “nomeDestinatario“

Você utilizará a API gratuita de consulta de CEP abaixo: 
Documentação da API: https://viacep.com.br/
Exemplo do GET: https://viacep.com.br/ws/<CEP_A_CONSULTAR>/json/

Endpoint pode ser público
Response/Output deve possuir: “vlTotalFrete” e “dataPrevistaEntrega”, “cepOrigem” e “cepDestino”
Deve ser persistido no banco os valores da cotação os valores consultados: “peso”, “cepOrigem”, “cepDestino”, “nomeDestinatario”, “vlTotalFrete”, “dataPrevistaEntrega” e “dataConsulta”

## Requisitos do sistema
 - Implementar apenas a API 
 - Versão Java +8 (caso seja Java 8, verificar compatibilidade da sua IDE)
 - Versão Spring Boot >= 2.4
Banco de dados fica a seu critério (Sql, NoSql)
Seu projeto deve obrigatoriamente ter as anotações: @Repository, @Entity e @Controller
Documentação mínima da API (Swagger ou documento PDF)

## Critérios de avaliação:
 * Implementação das regras de negócios para o cálculo do frete
 * Boas práticas de programação, arquitetura  e padrões de projetos


<h1 id="documentacao">
<img height="30" src="https://img.icons8.com/color/48/000000/documents.png"/>
  Documentação
</h1>

<p text-align="justify">Foi utilizado o swagger para criação da documentação automática da API. 


<h1 id="tecnologias-dependencias">
<img height="30" src="https://img.icons8.com/fluency/50/000000/administrative-tools.png"/>
	Tecnologias e Dependências
</h1>

<a name = "tech_stack"></a>

- Java 17 - Versão do Java utilizada
- Spring boot 2.6.3 - Framework de desenvolvimento
- Maven- Gerenciador de dependencias
- ViaCep - Api consumida para buscar os endereços
- H2 Database - Database para o ambiente de testes
- MySql Database - Database para o ambiente de produção
- Spring Data Jpa - Abstração orm do spring pra integração com o banco de dados
- Swagger - Documentação oficial da API
- Postman - Ferramenta para testes nas requisições
- Lombok - Framework para abstração e melhora na legibilidade do código
- ModelMapper - Facilitar o mapeamento de objetos e diminuir código boilerplate


<h1 id="desenvolvedor">
<img height="30" src="https://img.icons8.com/color/48/000000/devpost.png"/>
  Desenvolvedor
</h1>

<table align="center">
  <tr>
    <td align="center"><a href="https://github.com/oneyottabyte"><img style="border-radius: 50%;" src="https://avatars.githubusercontent.com/oneyottabyte" width="100px;" alt=""/><br /><sub><b>Dorian Vieira</b></sub></a><br /><a href="https://github.com/oneyottabyte" title="Dorian Vieira"></a></td>
  </tr>
</table>
