# PROPOSTA DE SOLUÇÃO PARA A FAST ENGINEERING S/A

## ESCOPO:
A **Fast Engineering S/A** busca uma solução para atender ao crescimento exponencial de seu eCommerce, com um aumento de 20% na demanda a cada mês. O escopo da solução inclui:

- Implantação de uma infraestrutura na AWS.
- Utilização de Kubernetes para gerenciar os servidores de aplicação REACT.
- Configuração de um banco de dados MySQL de alta disponibilidade no Amazon RDS.
- Armazenamento de recursos estáticos em Amazon EFS.
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

### Balanceamento de Carga com Healthcheck:

Configuraremos o Amazon Elastic Load Balancer (ELB) para distribuir o tráfego entre os servidores de aplicação, monitorando a saúde de cada instância por meio de healthchecks.

### Segurança (Liberar Somente o Necessário/Mínimo Acesso Possível):

Implementaremos medidas de segurança, como a utilização do AWS Identity and Access Management (IAM) para controlar o acesso aos recursos, Security Groups para restringir o tráfego de rede e Virtual Private Cloud (VPC) para isolar a infraestrutura.

### Considerações Adicionais:

Utilizaremos contêineres Docker para empacotar a aplicação REACT e suas dependências, permitindo a implantação eficiente no ambiente Kubernetes.

A arquitetura proposta é altamente escalável e pode lidar com o crescimento exponencial do eCommerce da "Fast Engineering S/A".

A integração contínua e a entrega contínua (CI/CD) podem ser implementadas para automatizar o processo de implantação e atualização da aplicação.


## VALORES:
Vemos depois com calma

## PRAZO DE ENTREGA:
24 de março de 2024.

# Cronograma Macro de Entregas

## Mês 1-2: Configuração do ambiente Kubernetes na AWS e migração da aplicação:

- **Semana 1-2:** (20/NOV/2023 - 03/DEZ/2023) Planejamento e preparação do ambiente EKS (Amazon Elastic Kubernetes Service) na AWS.
- **Semana 3-4:** (04/DEZ/2023 - 17/DEZ/2023) Criação do cluster Kubernetes, configuração dos servidores de aplicação REACT e migração da aplicação existente.
- **Semana 5-6:** (18/DEZ/2023 - 31/DEZ/2023) Testes iniciais de desempenho e funcionalidade do ambiente EKS.

## Mês 3-4: Implementação do Amazon RDS e configuração do Amazon EBS:

- **Semana 7-8:** (01/JAN/2024 - 14/JAN/2024) Configuração do Amazon RDS (Relational Database Service) para o banco de dados MySQL, incluindo provisionamento de recursos e configuração de segurança.
- **Semana 9-10:** (15/JAN/2024 - 28/JAN/2024) Configuração do Amazon Elastic Block Store (EBS) para armazenamento de recursos necessários.
- **Semana 11-12:** (29/JAN/2024 - 11/FEV/2024) Integração dos servidores de aplicação REACT com o banco de dados RDS e testes de conectividade e desempenho.

## Mês 5-6: Configuração de políticas de backup e medidas de segurança na AWS:

- **Semana 13-14:** (12/FEV/2024 - 25/FEV/2024) Implementação de políticas de backup automático no Amazon RDS e configuração de retenção de dados.
- **Semana 15-16:** (26/FEV/2024 - 10/MAR/2024) Refinamento das políticas de segurança, incluindo o uso de AWS Identity and Access Management (IAM) e outras medidas de controle de acesso.
- **Semana 17-18:** (11/MAR/2024 - 24/MAR/2024) Testes abrangentes de segurança e backup para garantir a integridade dos dados e a proteção contra ameaças.
