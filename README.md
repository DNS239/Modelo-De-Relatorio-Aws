# Relatorio-De-Implementação-De-Serviços-Aws

Data: 21/05/2024
Empresa: Absterco Industries
Responsavel: Denis Ajala

## Introdução
Essas ferramentas permitem uma gestão robusta e eficiente de todo o ciclo de vida do desenvolvimento de software, aproveitando a infraestrutura escalável e segura da AWS.

## Descriçao Do Projeto
Etapa 1: 
- AWS CodeCommit
- Foco da ferramenta: Controle de Versão
 -Descrição de caso de uso: AWS CodeCommit é um serviço de controle de versão que hospeda repositórios Git seguros na AWS. Os desenvolvedores podem usar CodeCommit para armazenar e versionar o código-fonte, colaborar com a equipe e rastrear alterações no código. Ele é totalmente gerenciado e se integra com outras ferramentas da AWS, facilitando a segurança e a escalabilidade.

Etapa 2: 
- AWS CodeBuild
- Foco da ferramenta: Integração Contínua (CI)
- Descrição de caso de uso: AWS CodeBuild é um serviço de construção contínua totalmente gerenciado que compila o código-fonte, executa testes e produz artefatos de software prontos para implantação. Sempre que há uma alteração no repositório CodeCommit, CodeBuild pode ser acionado automaticamente para compilar e testar o código, garantindo que ele funcione corretamente antes de ser mesclado ou implantado.

Etapa 3: 
- AWS CodeDeploy
- Foco da ferramenta: Entrega Contínua (CD)
- Descrição de caso de uso: AWS CodeDeploy é um serviço que automatiza a implantação de código para qualquer instância, seja Amazon EC2, AWS Lambda ou servidores on-premises. Ele permite realizar implantações automatizadas e coordenadas de maneira eficiente e segura, minimizando o tempo de inatividade e evitando erros manuais. CodeDeploy pode ser integrado com CodeCommit e CodeBuild para criar um pipeline CI/CD completo.

Essas ferramentas AWS são projetadas para funcionar perfeitamente em conjunto, proporcionando um fluxo de trabalho contínuo e eficiente do desenvolvimento à produção.

## Fluxo de Trabalho Proposto:
Desenvolvimento e Controle de Versão (CodeCommit): Os desenvolvedores fazem commit e push do código para repositórios CodeCommit.
Integração Contínua (CodeBuild): Cada commit aciona CodeBuild para compilar e testar o código automaticamente.
Entrega Contínua (CodeDeploy): Após a aprovação nos testes, CodeDeploy implanta o código nas instâncias designadas, garantindo que as novas versões sejam lançadas de maneira segura e eficiente.
