# DynamoDB
## Atividade: 
<p>A empresa de exploração espacial Space X é uma das pioneiras no mercado. Existe uma API (que não é filiada da empresa) que disponibiliza dados com informações de foguetes, viagens, lançamentos, etc. Vamos consultar essa API e gravar os dados nos recursos s3 e DynamoDB da AWS. Via API. Utilizando Python.</p>
<p><i>API = https://api.spacexdata.com/v3</i></p>

#### 1 - Crie um bucket no s3 com o nome spacex-21052020 - (Nesse bucket vamos gravar os dados no formato ‘.json’).
#### 2 - Crie as 3  tabelas abaixo no dynamodb:
<p><b>Tabela 1:</b> 
<ol>
  <li>Nome da Tabela: = capsule</li>
  <li>Chaves Hash: capsule_serial (tipo string)</li>
  <li>Chaves Range = capsule_id (tipo string)</li>
</ol>

<p><b>Tabela 2:</b> 
<ol>
  <li>Nome da Tabela: = rocket</li>
  <li>Chaves Hash: id (tipo number)</li>
  <li>Chaves Range = name (tipo string)</li>
</ol>

<p><b>Tabela 3:</b> 
<ol>
  <li>Nome da Tabela: = dragon</li>
  <li>Chaves Hash: id (tipo number)</li>
  <li>Chaves Range = name (tipo string)</li>
</ol>


#### 3 - Inserir dados da API relacionadas abaixo nos bancos do dynamodb e pasta indicadas no bucket criado no exercício 1:

<ol>
  <li>Capsule</li>
  <li>API: https://api.spacexdata.com/v3/capsules</li>
  <li>Tabela do Dynamodb: capsule</li>
  <li>Diretório do Bucket do S3: capsules/capsules.json</li>
</ol>
<p>_______________________________________________________________</p>

<ol>
  <li>Rockets</li>
  <li>API: https://api.spacexdata.com/v3/rockets</li>
  <li>Tabela do Dynamodb: rocket</li>
  <li>Diretório do Bucket do S3: rockets/rockets.json</li>
</ol>
<p>_______________________________________________________________</p>

<ol>
  <li>Dragons</li>
  <li>API: https://api.spacexdata.com/v3/dragons</li>
  <li>Tabela do Dynamodb: dragon</li>
  <li>Diretório do Bucket do S3: dragons/dragons.json</li>
</ol>
