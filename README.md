# Processamento de Dados Simplificado com Power BI e MySQL

Este projeto faz parte de um desafio da DIO para extração, transformação e modelagem de dados.

## 🛠️ Tecnologias Utilizadas
* **Banco de Dados:** MySQL (via XAMPP)
* **Ferramenta de BI:** Power BI Desktop
* **Linguagem de Consulta:** SQL e M (Power Query)

## 🚀 Adaptação Técnica
Diferente da proposta original usando Azure, este projeto foi implementado em ambiente **local** utilizando o **XAMPP**. 
* **Porta:** 3308
* **Driver:** MySQL Connector/NET 8.0.28

## 🔄 Etapas de Transformação (Power Query)
1. **Limpeza de Endereço:** Divisão da coluna `Address` em Número, Logradouro, Cidade e Estado.
2. **Nomes Unificados:** Mescla dos campos `Fname`, `Minit` e `Lname` para criar o `Nome Completo`.
3. **Hierarquia:** Criação de relação de gerência através de Self-Join.
4. **Relacionamentos:** Integração das tabelas de Departamentos com Localizações e Projetos.
5. **Modelagem Star Schema:** Organização das tabelas em Dimensões e Fatos para melhor performance.

## 📊 Visualização do Modelo
![Modelo Estrela](Imagens/seu_print_do_modelo.png)

## 📎 Como reproduzir
1. Execute o script SQL da pasta `/SQL` no seu MySQL.
2. Abra o arquivo `.pbix` na pasta `/PowerBI`.
3. Caso necessário, altere as configurações de fonte de dados para o seu servidor local.
