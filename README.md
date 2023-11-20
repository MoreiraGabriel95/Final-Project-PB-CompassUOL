# PROPOSTA DE SOLUÇÃO PARA A FAST ENGINEERING S/A

## ESCOPO:
A **Fast Engineering S/A** busca uma solução para atender ao crescimento exponencial de seu eCommerce, com um aumento de 20% na demanda a cada mês. O escopo da solução inclui:

- Implantação de uma infraestrutura na AWS.
- Utilização de Kubernetes para gerenciar os servidores de aplicação REACT.
- Configuração de um banco de dados MySQL de alta disponibilidade no Amazon RDS.
- Armazenamento de recursos estáticos em Amazon S3.
- Implementação de segurança com AWS IAM.
- Configuração de backups automáticos no Amazon RDS.
- Monitoramento e manutenção contínua.

## Arquitetura Proposta

### Ambiente Kubernetes:

Utilizaremos o Amazon Elastic Kubernetes Service (EKS) para gerenciar o ambiente Kubernetes, proporcionando escalabilidade e gerenciamento eficiente dos contêineres.

### Banco de Dados:

Optaremos por usar o Amazon RDS com a opção MySQL como banco de dados gerenciado, oferecendo recursos de alta disponibilidade, escalabilidade e gerenciamento simplificado.

### MultiAZ:

Configuraremos o Amazon RDS Multi-AZ para garantir redundância e alta disponibilidade do banco de dados em diferentes zonas de disponibilidade.

### Segurança de Backup de Dados:

Implementaremos backups automáticos no Amazon RDS MySQL, garantindo a recuperação dos dados em caso de falhas.

### Persistência dos Dados:

Utilizaremos armazenamento persistente do Amazon EBS (Elastic Block Store) para garantir a persistência dos dados dos contêineres.

### Armazenamento Estático:

Recursos estáticos, como imagens e arquivos CSS, serão armazenados no Amazon S3 para garantir escalabilidade e eficiência no carregamento.

### Balanceamento de Carga com Healthcheck:

Configuraremos o Amazon Elastic Load Balancer (ELB) para distribuir o tráfego entre os servidores de aplicação, monitorando a saúde de cada instância por meio de healthchecks.

### Segurança (Liberar Somente o Necessário/Mínimo Acesso Possível):

Implementaremos medidas de segurança, como a utilização do AWS Identity and Access Management (IAM) para controlar o acesso aos recursos, Security Groups para restringir o tráfego de rede e Virtual Private Cloud (VPC) para isolar a infraestrutura.

### Considerações Adicionais:

Utilizaremos contêineres Docker para empacotar a aplicação REACT e suas dependências, permitindo a implantação eficiente no ambiente Kubernetes.

A arquitetura proposta é altamente escalável e pode lidar com o crescimento exponencial do eCommerce da "Fast Engineering S/A".

A integração contínua e a entrega contínua (CI/CD) podem ser implementadas para automatizar o processo de implantação e atualização da aplicação.


## VALORES:
Detalhado no ppt.

## PRAZO DE ENTREGA:
Detalhado no ppt.

# Cronograma Macro de Entregas

## Configuração do ambiente Kubernetes na AWS e migração da aplicação:

- Planejamento e preparação do ambiente EKS (Amazon Elastic Kubernetes Service) na AWS.
- Criação do cluster Kubernetes, configuração dos servidores de aplicação REACT e migração da aplicação existente.
- Testes iniciais de desempenho e funcionalidade do ambiente EKS.

## Implementação do Amazon RDS e configuração do Amazon EBS:

- Configuração do Amazon RDS (Relational Database Service) para o banco de dados MySQL, incluindo provisionamento de recursos e configuração de segurança.
- Configuração do Amazon Elastic Block Store (EBS) para armazenamento de recursos necessários.
- Integração dos servidores de aplicação REACT com o banco de dados RDS e testes de conectividade e desempenho.

## Configuração de políticas de backup e medidas de segurança na AWS:

- Implementação de políticas de backup automático no Amazon RDS e configuração de retenção de dados.
- Refinamento das políticas de segurança, incluindo o uso de AWS Identity and Access Management (IAM) e outras medidas de controle de acesso.
- Testes abrangentes de segurança e backup para garantir a integridade dos dados e a proteção contra ameaças.
