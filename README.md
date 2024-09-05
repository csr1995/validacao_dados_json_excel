# Conversão e Validação de Dados de Excel para JSON

Este projeto realiza a conversão de dados de um arquivo Excel para o formato JSON, valida as informações, e processa os dados para atualizar uma base existente. O fluxo inclui a leitura e conversão dos dados, validação dos mesmos e geração de arquivos de saída com informações processadas, incluindo erros e atualizações.

## Funcionalidades ##

1. **Conversão de XLSX para JSON:**
   
   - Lê dados de um arquivo Excel (.xlsx) e converte para um formato JSON estruturado.
   - Valida e formata a data de nascimento e outros campos de acordo com o padrão definido.
     
2. **Validação dos Dados:**
   
   - Valida CPF, e-mail, telefone, data de nascimento e CEP.
   - Gera um relatório de erros para dados inválidos.
     
3. **Atualização de Dados:**
   
   - Compara dados novos com uma base existente.
   - Classifica os dados como novos ou atualizados.
   - Salva os dados novos e atualizados em arquivos separados.
     
4. **Relatório de Erros:**
   
   - Gera um arquivo Excel com os clientes que possuem erros de validação.

## Uso ##

1. **Conversão de XLSX para JSON**

   - Chame a função xlsx_para_json passando o caminho do arquivo XLSX e o caminho do arquivo JSON de destino.
  
2. **Processamento e Validação de Dados**

   - Chame a função processar_json passando o caminho do arquivo JSON e o caminho do arquivo Excel da base de dados.
  
   ![image](https://github.com/user-attachments/assets/5d682c63-fbaf-423c-9fcc-b3a540d6b5a0)

## Estrutura dos Arquivos ##

   - **dados.xlsx**: Arquivo Excel com os dados a serem convertidos.
   - **dados.json**: Arquivo JSON gerado a partir do Excel.
   - **novos_clientes.json**: Arquivo JSON com novos clientes.
   - **atualizacao_clientes.json**: Arquivo JSON com clientes a serem atualizados.
   - **clientes_com_erros.xlsx**: Arquivo Excel com clientes que possuem erros.

## Funções Utilizadas ##

   - xlsx_para_json(caminho_xlsx, caminho_json): Converte o arquivo Excel em JSON.
   - validar_cpf(cpf): Valida um CPF.
   - validar_data_nascimento(data_nascimento): Valida a data de nascimento.
   - validar_email(email): Valida um e-mail.
   - validar_telefone(ddd, telefone): Valida um telefone.
   - validar_cep(cep): Valida um CEP.
   - ler_base_excel(caminho_arquivo): Lê a base de dados do arquivo Excel.
   - atualizar_dados(novos_dados, base_dados): Atualiza a base de dados com novos dados.
   - processar_cliente(dados): Processa e valida um cliente.
   - processar_json(caminho_json, caminho_excel): Processa o arquivo JSON e atualiza a base de dados.

