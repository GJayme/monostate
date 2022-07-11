# Monostate:

## O que é?
Nesse padrão o construtor da classe <strong>ConnectionPool</strong> está público, ou seja, nós conseguimos criar quantas instâncias forem necessárias e temos acesso direto ao método <strong>getConnection</strong>.

O que acaba mudando em relação o Singleton é que o <strong>pool</strong> de conexões, que nesse exemplo é uma agregação, ou seja, podemos utilizar o <strong>Connection</strong> sem ter a pool de conexões. O fato é que a variável pool é um elemento estático e isso faz com que nós temos um único ESTADO. O Estado é compartilhado entre todas as instâncias. A GRANDE VANTAGEM disso é que conseguimos utilizar interfaces.

## Observações:
