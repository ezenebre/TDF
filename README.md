# TDF
ABAP developments for SAP TDF (Tax Declaration Framework)

### ZCL_TOM ###

Portuguese:

A classe ZCL_TOM foi desenvolvida para facilitar o uso da TOM API no SAP TDF afim de disponibilizar arquivos gerados através de desenvolvimentos ABAP no TOM (Tax Obligation Monitor). Para a implementação desta classe, é necessário realizar a configuração da obrigação fiscal através da transação SPRO no ambiente TDF e informar os parâmetros abaixo:

IV_REPORT_ID (Report ID criado na configuração na SPRO);
IV_EMPRESA (Código da Empresa);
IV_FILIAL (Código da Filial);
IV_CNPJ_ROOT (Raiz de CNPJ, pode ser encontrada na tabela /TMF/D_CNPJ_ROOT);
IV_DT_INI (Data inicial do arquivo no formato AAAAMMDD);
IV_DT_FIN (Data final do arquivo no formato AAAAMMDD);
IT_FILE (Conteúdo do arquivo, é necessário apenas alimentar o campo REG da estrutura /TMF/S_SPED_OUTPUT. Os demais campos são desnecessários);

English:

The class ZCL_TOM was developed to facilitate the use of the TOM API from SAP TDF to create available ABAP developed files in TOM (Tax Obligation Monitor). For class implementation, you need to create a new fiscal report in SPRO transaction and insert the follow parameters:

IV_REPORT_ID (Report ID created by SPRO configuration);
IV_EMPRESA (Company Code);
IV_FILIAL (Business Place);
IV_CNPJ_ROOT (CNPJ Root, you can found in /TMF/D_CNPJ_ROOT table);
IV_DT_INI (Initial file date in YYYYMMDD format);
IV_DT_FIN (Final file date in YYYYMMDD format);
IT_FILE (The file content. You need APPEND just the REG field of structure /TMF/S_SPED_OUTPUT. Another fields are unnecessary);
