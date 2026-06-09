# Projeto-5-semestre---Java-Decorator---Design-Petterns
Sistema web desenvolvido em Java com JSP, Servlets, JDBC e MySQL para gerenciamento de pedidos de açaí. Utiliza o padrão de projeto Decorator para permitir a personalização dinâmica dos produtos com diferentes complementos, além de carrinho de compras, cálculo automático de valores e registro de pedidos.
# 🍧 AçaíMix

Sistema web desenvolvido em Java para gerenciamento de pedidos de uma loja de açaí, permitindo que os clientes personalizem seus produtos com diferentes tamanhos e complementos.

## 📌 Sobre o Projeto

O AçaíMix foi desenvolvido como projeto acadêmico com o objetivo de aplicar conceitos de Programação Orientada a Objetos, arquitetura MVC, persistência de dados com JDBC e o padrão de projeto **Decorator**.

A aplicação permite que o cliente monte seu próprio açaí, escolhendo o tamanho desejado e adicionando complementos, calculando automaticamente o valor final do produto.

## 🚀 Funcionalidades

* Seleção do tamanho do açaí

  * Pequeno
  * Médio
  * Grande

* Adição de complementos

  * Granola
  * Manga
  * Nutella
  * Paçoca
  * Leite Condensado

* Carrinho de compras

* Remoção de itens do carrinho

* Cálculo automático do valor total

* Escolha da forma de pagamento

* Registro dos pedidos em banco de dados

* Consulta dos pedidos cadastrados

## 🏗️ Padrões Utilizados

### Decorator

O padrão Decorator foi utilizado para adicionar complementos aos açaís de forma dinâmica, sem a necessidade de criar inúmeras combinações de classes.

Exemplo:

Açaí Grande → Nutella → Granola → Manga

Cada complemento adiciona sua descrição e valor ao produto final.

## 🛠️ Tecnologias Utilizadas

* Java
* JSP
* Servlets
* JDBC
* MySQL
* Apache Tomcat
* HTML
* CSS
* NetBeans IDE

## 📂 Estrutura do Projeto

* Model

  * Pedido
  * Alimento
  * AcaiPequeno
  * AcaiMedio
  * AcaiGrande
  * AdicionaisDecorator
  * Granola
  * Manga
  * Nutella
  * Paçoca
  * LeiteCondensado

* DAO

  * PedidoDAO

* Controller

  * PedidoController

* Views (JSP)

  * index.jsp
  * adicionais.jsp
  * carrinho.jsp
  * pagamento.jsp
  * pagamentoFinalizado.jsp

## 🗄️ Banco de Dados

Tabela principal utilizada para armazenamento dos pedidos:

```sql
CREATE TABLE pedido (
    id INT AUTO_INCREMENT PRIMARY KEY,
    descricao VARCHAR(500),
    dataPedido DATETIME NOT NULL,
    valorTotal DECIMAL(10,2) NOT NULL,
    pagamento VARCHAR(50),
    status VARCHAR(30)
);
```

## ▶️ Como Executar

1. Clonar o repositório.
2. Importar o projeto no NetBeans.
3. Configurar o Apache Tomcat.
4. Criar o banco de dados MySQL.
5. Executar o script SQL.
6. Configurar a conexão JDBC.
7. Executar o projeto.

## 👨‍💻 Autor

Felipe Santana Carvalho Ribeiro Furtado
Igor da Silva Neves
Matheus Carvalho

Projeto desenvolvido para fins acadêmicos na disciplina de Engenharia de Software.
