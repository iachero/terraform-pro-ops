# Roteiro de Estudos para Certificação Terraform Authoring and Operations Pro com AWS 🚀

## 1. Introdução 📋

Este roteiro de estudos foi criado para ajudar na preparação para o exame de certificação Terraform Authoring and Operations Professional com AWS. O exame avalia conhecimentos avançados em configuração e fluxos de trabalho do Terraform em ambientes de produção.

## 2. Pré-requisitos 🔍

- Certificação HashiCorp Terraform Associate (recomendado)
- Habilidades básicas de Linux (navegação, edição de arquivos, permissões)
- Experiência com formatos YAML, JSON, HCL e CSV
- Conhecimento de redes e protocolos (TCP/IP, UDP)
- Experiência com o provider AWS do Terraform em ambiente de produção
- Conhecimento de credenciais em nuvem

## 3. Formato do Exame 📝

- **Versão do Terraform**: 1.6
- **Ambiente**: Linux pré-configurado
- **Tipos de questões**:
  - Cenários práticos (labs) - Modificação de configurações e provisionamento de infraestrutura real
  - Questões de múltipla escolha

Durante o exame, você terá acesso à documentação do Terraform, documentação do provider AWS e console AWS, mas não poderá acessar tutoriais HashiCorp ou recursos externos.

## 4. Objetivos do Exame 🎯

### 4.1 Gerenciar o ciclo de vida dos recursos

- Inicialização de configurações (`terraform init`)
- Geração de planos de execução (`terraform plan`)
- Aplicação de mudanças (`terraform apply`)
- Destruição de recursos (`terraform destroy`)
- Gerenciamento de estado (importação, reconciliação de drift)

### 4.2 Desenvolver e solucionar problemas em configurações dinâmicas

- Validação de configurações com recursos da linguagem
- Consulta a providers usando data sources
- Computação e interpolação de dados usando funções HCL
- Uso de meta-argumentos em configurações
- Configuração de variáveis de entrada e saídas, incluindo tipos complexos
- Melhores práticas para gerenciar dados sensíveis

### 4.3 Desenvolver fluxos de trabalho colaborativos do Terraform

- Gerenciamento de versões de módulos, providers e binário do Terraform
- Configuração e uso de estado remoto
- Compartilhamento de dados entre configurações e arquivos de estado
- Modificação de fluxos de trabalho para automação

### 4.4 Criar, manter e usar módulos do Terraform

- Criação de módulos
- Uso de módulos em configurações
- Refatoração de módulos e versionamento
- Refatoração de configurações existentes em módulos

### 4.5 Configurar e usar providers

- Arquitetura baseada em plugins do Terraform
- Configuração de providers (aliasing, versionamento, origem)
- Gerenciamento de autenticação de providers
- Solução de problemas com providers

### 4.6 Colaborar usando HCP Terraform (apenas questões de múltipla escolha)

- Fluxo de trabalho do HCP Terraform
- Workspaces do HCP Terraform e opções de configuração
- Gerenciamento de credenciais de providers no HCP Terraform
- Policy as code e recursos de governança

## 5. Recursos AWS para Revisar 🌐

- aws_instance
- aws_ami (data source)
- aws_launch_template
- aws_autoscaling_group
- aws_security_group
- aws_security_group_rule
- aws_s3_object
- random_integer
- aws_s3_bucket
- aws_caller_identity (data source)
- aws_iam_session_context (data source)
- aws_iam_policy_document (data source)
- aws_iam_role
- aws_subnet (data source)
- aws_vpc_security_group_ingress_rule
- aws_iam_instance_profile
- aws_iam_policy
- aws_iam_role_policy_attachment
- Backend S3 do Terraform
- terraform_remote_state (data source com backend S3)

## 6. Plano de Estudos Detalhado 📚

### Semana 1-2: Fundamentos e Ciclo de Vida dos Recursos

- Revisão dos comandos básicos do CLI (init, plan, apply, destroy)
- Estudo aprofundado sobre gerenciamento de estado
- Prática com importação de recursos e reconciliação de drift
- Exercícios de refatoração de configurações

### Semana 3-4: Configurações Dinâmicas

- Estudo de funções HCL e expressões
- Prática com data sources
- Implementação de meta-argumentos (count, for_each, depends_on, lifecycle)
- Configuração de variáveis complexas e outputs
- Gerenciamento de dados sensíveis

### Semana 5-6: Módulos e Fluxos de Trabalho Colaborativos

- Criação e uso de módulos
- Versionamento de módulos
- Configuração de estado remoto
- Compartilhamento de dados entre configurações
- Automação de fluxos de trabalho do Terraform

### Semana 7-8: Providers e HCP Terraform

- Configuração avançada de providers
- Aliasing de providers
- Métodos de autenticação
- Estudo sobre HCP Terraform
- Workspaces e configurações
- Policy as code

## 7. Recursos de Estudo 📖

### Documentação Oficial
- [Documentação do Terraform](https://developer.hashicorp.com/terraform/docs)
- [Documentação do Provider AWS](https://registry.terraform.io/providers/hashicorp/aws/latest/docs)

### Tutoriais Recomendados
- [Gerenciar ciclo de vida de recursos](https://developer.hashicorp.com/terraform/tutorials/state/resource-lifecycle)
- [Usar count](https://developer.hashicorp.com/terraform/tutorials/configuration-language/count)
- [Usar for_each](https://developer.hashicorp.com/terraform/tutorials/configuration-language/for-each)
- [Criar expressões dinâmicas](https://developer.hashicorp.com/terraform/tutorials/configuration-language/expressions)
- [Variáveis sensíveis](https://developer.hashicorp.com/terraform/tutorials/configuration-language/sensitive-variables)
- [Criar e usar módulos locais](https://developer.hashicorp.com/terraform/tutorials/modules/module-create)
- [Usar módulos públicos](https://developer.hashicorp.com/terraform/tutorials/modules/module-use)
- [Refatorar configuração monolítica](https://developer.hashicorp.com/terraform/tutorials/modules/organize-configuration)

## 8. Dicas para o Exame 💡

- Pratique em um ambiente Linux real
- Familiarize-se com a sintaxe HCL avançada
- Entenda profundamente o ciclo de vida dos recursos
- Pratique a refatoração de código e migração de estado
- Estude os padrões de design de módulos
- Compreenda as opções de configuração de providers
- Pratique a solução de problemas comuns

## 9. Melhores Práticas 🛡️

- Use controle de versão para suas configurações
- Implemente validação de configuração
- Utilize módulos para código reutilizável
- Gerencie adequadamente dados sensíveis
- Implemente testes para suas configurações
- Documente seu código adequadamente
- Siga as convenções de nomenclatura

## 10. Considerações de Segurança 🔒

- Proteja seus arquivos de estado
- Use variáveis sensíveis para dados confidenciais
- Implemente o princípio do menor privilégio para IAM
- Considere o uso do HashiCorp Vault para gerenciamento de segredos
- Implemente políticas de segurança como código