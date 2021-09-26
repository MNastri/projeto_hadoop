# projeto_hadoop
*Projeto parte do módulo "Criando um ecossistema Hadoop totalmente gerenciado com Google Cloud Dataproc"*

## Objetivo
Ler as linhas do documento ```livro.txt``` fornecido pelo curso e retornar uma lista ```resultado.txt``` com as 10 palavras mais utilizadas neste documento. Incluir no repositório o arquivo ```part-00000``` com toda a lista de palavras e sua frequência no texto.

## Resolução
1. Criamos o ecossistem na Google Cloud Platform (GCP) com bucket e cluster dataproc.
2. Executamos o job do tipo PySpark chamando o código fonte ```contador.py``` fornecido pelo curso, após realizarmos as devidas alterações necessárias para o nosso caso.
3. Criado o documento ```resultado.txt``` com as 10 palavras mais frequentes.
4. Arquivos ```resultado.txt``` e ```part-00000``` adicionados ao repositório.
