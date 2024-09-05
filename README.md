# Conversão e Validação de Dados de Excel para JSON

Este projeto realiza a conversão de dados de um arquivo Excel para o formato JSON, valida as informações, e processa os dados para atualizar uma base existente. O fluxo inclui a leitura e conversão dos dados, validação dos mesmos e geração de arquivos de saída com informações processadas, incluindo erros e atualizações.

## Funcionalidades ##

1. **Conversão de XLSX para JSON:**
   
   - Lê dados de um arquivo Excel (.xlsx) e converte para um formato JSON estruturado.
   - Valida e formata a data de nascimento e outros campos de acordo com o padrão definido.
   - 
2. **Validação dos Dados:**
   
   - Valida CPF, e-mail, telefone, data de nascimento e CEP.
   - Gera um relatório de erros para dados inválidos.
   - 
3. **Atualização de Dados:**
   
   - Compara dados novos com uma base existente.
   - Classifica os dados como novos ou atualizados.
   - Salva os dados novos e atualizados em arquivos separados.
   - 
4. **Relatório de Erros:**
   
   - Gera um arquivo Excel com os clientes que possuem erros de validação.

