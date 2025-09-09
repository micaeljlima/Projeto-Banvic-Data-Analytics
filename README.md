# Projeto de Análise de Dados do Banco Vitória
![banner](readme/banvic_logo.jpeg)

## Introdução:
Este projeto tem como foco a construção de um painel interativo no Power BI, como produto final, passando por etapas de pré-processamento, manipulação, modelagem e visualização de dados. Os dados utilizados pertencem a um banco fictício chamado Banco Vitória (ou “Banco Vic”).

## Arquitetura do Projeto:

![arquitetura_projeto](readme/Arquitetura_BanVic.gif)

## Justificativa:

No início, a instituição enfrenta diversos problemas relacionados à governança de dados, estando presa a métodos ultrapassados e a uma cultura conservadora entre os colaboradores. Diante desse cenário, surgiu a proposta deste projeto: apresentar um novo ponto de vista sobre como os dados podem ser trabalhados dentro da empresa, de forma mais moderna, eficiente e estratégica.

## Tecnologias Utilizadas:

<div align="center" style="display: inline_block">
  <img align="center" alt="github" src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  <img align="center" alt="vscode" src="https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white" /> 
  <img align="center" src="https://img.shields.io/badge/Jupyter_Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="icon jupyter notebook">
  <img align="center" src="https://img.shields.io/badge/Python-133DAB?style=for-the-badge&logo=python&logoColor=white" alt="icon python">
  <img align="center" src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="icon pandas">
  <img align="center" src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="icon power bi">
  <img align="center" src="https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white" alt="icon figma">
  <img align="center" src="https://img.shields.io/badge/Canva-00C4CC?style=for-the-badge&logo=canva&logoColor=white" alt="icon canva">
</div>

## Datasets e seus Atributos:

| Dataset             | Variáveis                                                                                                                                                                                                                                                       | Descrição                                                                 |
|---------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------|
| Agencia             | cod_agencia, nome, endereco, cidade, uf, data_abertura, tipo_agencia                                                                                                                                                                                            | Informações sobre as agências bancárias. |
| Cliente             | cod_cliente, primeiro_nome, ultimo_nome, nome_completo, email, tipo_cliente, data_inclusao, cpfcnpj, data_nascimento, endereco, cep                                                                                                                              | Dados cadastrais e de identificação dos clientes.                |
| Colaborador_Agencia | cod_colaborador, cod_agencia                                                                                                                                                                                                                                    | Relação entre colaboradores e as agências em que trabalham.                 |
| Colaboradores       | cod_colaborador, primeiro_nome, ultimo_nome, nome_completo, email, cpf, data_nascimento, endereco, cep                                                                                                                                                           | Informações pessoais e de contato dos colaboradores.                        |
| Contas              | num_conta, cod_cliente, cod_agencia, cod_colaborador, tipo_conta, data_abertura, saldo_total, saldo_disponivel, data_ultimo_lancamento                                                                                                                           | Informações sobre contas bancárias. |
| Proposta_Credito    | cod_proposta, cod_cliente, cod_colaborador, data_entrada_proposta, taxa_juros_mensal, valor_proposta, valor_financiamento, valor_entrada, valor_prestacao, quantidade_parcelas, carencia, status_proposta                                                        | Propostas de crédito solicitadas por clientes. |
| Transacoes          | cod_transacao, num_conta, data_transacao, nome_transacao, valor_transacao                                                                                                                                                                                       | Registro de movimentações financeiras realizadas nas contas. |
| Clientes_Externos   | Numero_Linha, ID_Cliente, Sobrenome, Pontuação_Credito, Pais, Genero, Idade, Tempo_Relacionamento, Saldo, Numero_Produtos, Possui_Cartao_Credito, Membro_Ativo, Salario_Estimado, Saiu, Reclamou, Pontuaçao_Satisfaçao, Tipo_Cartao, Pontos_Acumulados           | Dataset externo com informações complementares de clientes de outro banco. |
