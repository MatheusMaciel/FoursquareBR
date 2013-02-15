FoursquareBR
============

Tutorial de execução dos scripts

a)	Ordem dos scripts:
1-	coleta_REST_API.php
Resultado = arquivos no formato .json em tempo real de cada cidade pela API do Twiter.

2-	teste.php
OBS = pelo script os arquivos estão dentro de uma pasta chamada med. Posso alterar de acordo com a minha configuração.
Resultado = transformar em .csv dos .json na etapa 1

3-	teste3.php 
Antes de executar o script = criar a pasta Atualidade_info e ID_info 
Resultados = arquivos .json com os IDs dos locais e outro arquivo .json com as atualidades (necessário para o cálculo da Atualidade)

4-	coleta.php 
OBS = Será essencial para o cálculo da Atualidade
OBS = olhar se o PATH das pastas Atualidade_info e ID_info estão corretas no script
Antes de executar os scripts = criar a pasta Datas
Resultado = arquivos .csv com as Datas de cada Local  (necessário para o cálculo da Atualidade)

5-	Executa o script em R 
Antes de executar os scripts = crie a pasta infoATT 
Resultado = gerar arquivos xls na pasta infoATT com os timestamps das marcações realizadas nos locais da cidade (necessário para o cálculo da Atualidade)

6-	CalcularAtualidade.php
OBS = confira o PATH de onde os csv com as taxas da atualidade serão salvos ... será necessário adequar a sua organização (no script está ./coletas/coleta3/atualidade/)
Resultado = arquivo .csv com a taxa de Atualidade dos locais da cidade.

7-	lerDenCor.php
Resultado = DensCobCid.csv (a cobertura e densidade de cada cidade).

OBS = até o momento forma calculadas as métricas de densidade, cobertura e atualidade.

Para calcular as métricas de atividade dos usuários e diversidade basta olhar o script em R junto com o artigo, ok?
