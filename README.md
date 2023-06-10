## Descrição

Exemplo de integração do RabbitMQ com aplicações Node.js usando Docker.

## Rodar o projeto

<p>
  Executar ```docker-compose up``` - Levanta todos os containers, inclusive o RabbitMQ. 
</p>

### Observação em relação ao Docker

<b> Atenção </b> - Devido a quebra de linha do Windows há o risco de ocorrer problemas ao rodar o ```docker-compose up``` acarretando na execução apenas do RabbitMQ e falha do Nest e Express. Para a correção disso é necessário configurar o padrão de quebra de linha do Git, para isso faça o seguinte:
```
git config --global core.autocrlf input

git rm --cached -r .
git reset --hard
```



### Testar a comunicação

* Com a extensão Rest Client do VSCode, abra o arquivo **rest.http** e faça requisições da aplicação Express ou Nest e verifique o retorno no console da aplicação contrária.
* Envie requisições POST para **http://localhost:3001/express** ou **http://localhost:3000/express** enviando um JSON no corpo da requisição e verifique o retorno no console da aplicação contrária.

## Créditos 
- O template base do projeto bem como parte de seu desenvolvimento é baseado em tutorial disponivel no <a href="https://www.youtube.com/@FullCycle"> Youtube da Full Cycle </a>

