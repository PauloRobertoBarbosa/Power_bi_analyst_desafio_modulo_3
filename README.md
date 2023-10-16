# Power_bi_analyst_desafio_modulo_3

#Preparação do Banco de dados
1) Criado instância no Microsoft Azure.
2) Criado banco de dados "teste" em Mysql.
3) Realizado integração entre Power Bi com o Mysql

#Transformação dos dados - 1º Parte

1) Verificar cabeçalho e tipos de dados:
   Tanto os cabeçalhos quanto os tipos de dados foram importados corretamente
2) Modificar valores monetários:
   Os valores monetários foram ajustados
3) Verificar existência de nulos:
   O único campo 'null' apresentado trata-se de gerente que não possui nenhum superior acima.
4) Verificar se há algum departamento sem gerente:
   Não há.

#Transformação dos dados - 2º Parte

1) Mesclar consultas employee e departament:
    Criado a mescla através do caminho:
      Power Query -> Página Inicial -> Mesclar Consultas:
<p align = "center">
  <img src = "https://user-images.githubusercontent.com/50236579/275478070-d5aa975e-a8bf-4f40-b622-3d4f7c0cb786.png">
</p>
   1.1) A opção de mescla permite buscar colunas de outras consultas desde que tenha alguma chave que valide os valores. (obs: acrescentar consultas iria adicionar linhas a base fazendo com que a leitura seja incorreta).

2) Criação de tabela de colaboradores e gerentes:
      Criado a mescla através do caminho:
      Power Query -> Página Inicial -> Mesclar Consultas:
      Mescla fazendo referência do Super_Ssn com o Ssn do employee:
<p align = "center">
  <img src = "https://user-images.githubusercontent.com/50236579/275478070-d5aa975e-a8bf-4f40-b622-3d4f7c0cb786.png">
</p>


