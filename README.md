# projeto_hadoop

## GCP Dataproc

__*Criando um ecossistema Hadoop totalmente gerenciado com Google Cloud Platform*__

O projeto consiste em efetuar um processamento de dados utilizando o produto Dataproc do GCP. Esse processamento irá efetuar a contagem das palavras de um livro e informar quantas vezes cada palavra aparece no mesmo.

---

### Etapas do projeto

1. Criar um bucket no Cloud Storage
2. Atualizar o arquivo ```contador.py``` com o nome do Bucket criado nas linhas que contém ```{SEU_BUCKET}```.
3. Fazer o upload dos arquivos ```contador.py``` e ```livro.txt``` para o bucket criado
4. Utilizar o código em um cluster Dataproc, executando um Job do tipo PySpark chamando ```gs://{SEU_BUCKET}/contador.py```
5. O Job irá gerar uma pasta no bucket chamada ```resultado```. Dentro dessa pasta o arquivo ```part-00000``` irá conter a lista de palavras e quantas vezes ela é repetida em todo o livro.

### Resultado

Verificar o arquivo chamado ```resultado.txt```. Dentro desse arquivo estão as 10 palavras que mais são usadas no livro, de acordo com o resultado do Job.

---

### Considerações Finais

NOTA: Se o Job mostrar um WARN de Interrupt, basta ignorar. Existe um bug no Hadoop que é conhecido. Isso não impacta no processamento.
