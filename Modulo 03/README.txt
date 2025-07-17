Respondendo as perguntas do desafio:

Pergunta 11:
Query SQL utilizada para realizar a junção dos colaboradores e respectivos nomes dos gerente:

SELECT 
  e.*,
  CONCAT(g.Fname, ' ', g.Minit, '.', ' ', g.Lname) AS ManagerName
FROM 
  employee e
LEFT JOIN 
  employee g ON e.Super_ssn = g.Ssn;


Pergunta 14 - Explique por que, neste caso supracitado, podemos apenas utilizar o mesclar e não o atribuir:

Mesclar colunas é usado quando você quer unir os valores de duas ou mais colunas em uma única coluna de texto, de forma direta e simples, 
usando um separador (como espaço, vírgula ou hífen). Por exemplo, juntar "Pesquisa" com "São Paulo" e formar "Pesquisa - São Paulo". 
É útil quando você só precisa exibir as informações juntas, sem lógica ou condições.

Já atribuir (criar) uma coluna personalizada permite mais controle. Você pode unir colunas também, mas com lógica condicional, 
cálculos ou formatos específicos. Por exemplo, adicionar “(SP)” ao nome do departamento apenas se a localização for “São Paulo”. 
Essa opção é mais flexível e poderosa, ideal quando você precisa aplicar regras ou personalizações no conteúdo.

