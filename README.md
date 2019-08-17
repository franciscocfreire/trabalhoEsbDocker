# Desafio Mule fiap

Esse desafio consiste em criar dois serviços da Web, usando REST.
Ambos devem ser criados no mesmo projeto usando o Anypoint Studio, o IDE para o Mule ESB  3.7 - IDE anypoint studio
Você pode baixá-lo em https://fiapcom-my.sharepoint.com/:u:/g/personal/pf0861_fiap_com_br/Ef07SrCfPnlFiYlT3-YY5u8B9CqWgDM7ttdPqI_TngrTEw?e=2ZKvbY. 
Certifique-se de usar a versão 3.7+ do Mule ESB.

Acreditamos que, sem qualquer experiência anterior com o Mule, você ainda poderá usá-lo devido ao seu IDE intuitivo. 
Se você tiver alguma dificuldade, verifique sua documentação (https://docs.mulesoft.com/mule-runtime/3.7/developing) e outros recursos como vídeos do YouTube.

Esta fonte contém o modelo básico para sua implementação.
O Mule 3.7+ e o Anypoint Studio são compatíveis apenas com o JDK 1.7+.

### 1 - Crie fluxo expondo EmpregadoFlow, um serviço REST, onde o cliente será capaz de:

* Inserir um empregado no banco
  * Recebe um funcionário e retorna uma mensagem de sucesso
* Listar todos os funcionários
  * payload vazio e retorna uma lista de funcionários

Seu serviço deve usar JSON como seu formato de representação para objetos.

Usar banco mysql criado via docker-compose.

Você deve definir os nomes dos recursos e os verbos HTTP usados de acordo com ODATA.


### 2 -  Crie fluxo expondo SalarioFlow, um serviço REST, onde o cliente será capaz de:


* Obter o salário médio dos empregados
  * Pedido vazio e retorna um decimal
* Calcular um bônus de funcionário
  * Recebe o ID do empregado e retorna o bônus como um decimal
  * O bônus deve ser uma porcentagem aleatória do salário do funcionário, mas não superior a 50%


### 3 - Crie um docker-compose e Dockerfile 

*Crie o Dockerfile e docker-compose.yaml e versione no bitbucket (como privado) e de acesso para o usuário daniboy1982

*suba os container com docker-compose up 

*teste os fluxos com postman e crie um PDF com todas as evidencias das execuções do postman e do fluxo no anypointstudio.

*inclua no pdf a url do repositorio do gitlab

*suba APENAS o pdf no portal!