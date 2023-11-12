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

## ARQUITETURA DA NOVA SOLUÇÃO:
1. **Balanceamento de Carga:**
   - Tráfego do usuário é direcionado para o Amazon Elastic Load Balancer (ELB) para distribuição equitativa entre os servidores de aplicação.

2. **Servidores de Aplicação REACT:**
   - Gerenciados em um cluster Kubernetes usando o Amazon Elastic Kubernetes Service (EKS).
   - Escalabilidade automática para lidar com picos de demanda.

3. **Banco de Dados MySQL:**
   - Hospedado no Amazon RDS para alta disponibilidade e redundância.
   - Configuração MultiAZ assegura continuidade do serviço.

4. **Armazenamento de Recursos Estáticos:**
   - Imagens, links e recursos estáticos são armazenados em Amazon EFS para eficiência e escalabilidade.

5. **Segurança:**
   - Controle de acesso gerenciado por AWS Identity and Access Management (IAM) para garantir a segurança dos recursos.
   - Princípio de acesso mínimo necessário.

6. **Autoescala:**
   - Kubernetes e Amazon RDS podem escalar automaticamente para atender ao aumento da demanda.

7. **Backups Automáticos:**
   - Amazon RDS realiza backups automáticos dos dados, garantindo a segurança.

8. **Monitoramento e Manutenção:**
   - AWS oferece ferramentas de monitoramento para acompanhar a saúde dos recursos e realizar manutenção.

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
