# Challenge

Solução desenvolvida a partir do .NET Framework 4.6.1 - Visual Studio 2015, com a finalidade de consumir e exibir dados a partir da Api Marvel Comics, que disponibiliza para desenvolvedores do mundo inteiro, o acesso a informações referente uma vasta biblioteca de quadrinhos de Super Heróis da Marvel que foi criada a 70 anos atrás.

De modo resumido, abaixo seguem alguns dos principais conceitos, técnicas, pacotes e tecnologias utilizadas/aplicadas neste projeto: 

## WEB

- Front End desenvolvido com o framework Angular JS, sendo implementado o Provider de autenticação de acesso OAuth 2.0, em comunicação com a Web Api Rest C#.

- Pacotes Web baixados via Bower.
	
## API
		
- Testes Unitários para simulação do comportamento esperado de uma respectiva ação em relação ao consumo à dados na Marvel Comics Api dentro da aplicação (conceito TDD).

- Estrutura em camadas, separação de responsabilidades, injeção de dependência, entre outros conceitos de SOLID e DDD.

- Uso do Banco de Dados Redis(NoSql), que possui a responsabilidade do armazenamento em cache dos dados em memória dentro da aplicação. O Redis foi consumido dentro do C# a partir da API **"NServiceKit.Redis"**, também baixada via NuGet.

	Comando via Package Manager Console: > **Install-Package NServiceKit.Redis**
	
- Foi aplicado o conceito de AOP através do pacote baixado via NuGet **“Postsharp”** para implementar aspector no C# em relação as Entidades que obtiveram seus dados armazenados em cache a partir de uma segunda requisição vinda do Client.

	Comando via Package Manager Console: > **Install-Package Postsharp**

## PUBLICAÇÃO

Aplicação publicada na Amazon, e disponível a partir dos seguintes links:

- WEB:
- API: 
