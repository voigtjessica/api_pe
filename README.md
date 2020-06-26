# API PE
Avaliação da API de Pernambuco para o projeto Tá na Mesa

* Informações da API estão disponíveis em: https://www.tce.pe.gov.br/internet/index.php/dados-abertos/definicoes-da-api
* Lista das bases com links para codebooks: https://sistemas.tce.pe.gov.br/DadosAbertos/Exemplo!listar

Observações:
* Não há informações sobre a capital, Recife.
* É possível filtrar por descrição do objeto incluindo "MERENDA" , mas o resultado trouxe licitações que não eram de merenda, então o jeito é fazer a requisição "inteira" e filtrar por merenda depois.
* Nas licitações estão disponíveis só os três últimos números do CPF do contratado, mas este dado está disponível na íntegra nos contratos. 
* Só é possível ver a quantidade e a descrição por item **na licitação** olhando o arquivo pdf do edital, considerei então que essa informação não está disponível. O mesmo vale para valor e quantidade estimada. 
* É possivel puxando vincular contrato à licitação pela API através dos campos AnoContrato + Processo (equivalente a  NUMEROPROCESSO na api das licitações)
* Existe na API a possibilidade de requisição de despesas, e verificar a liquidação e empenhos. No entanto, não é possível vincular diretamente ao contrato, mas sim a empresa.
