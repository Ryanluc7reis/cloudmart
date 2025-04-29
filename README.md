# CloudMart 🛒

<div align="center">
  
[![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)](https://aws.amazon.com/)
[![Azure](https://img.shields.io/badge/azure-%230072C6.svg?style=for-the-badge&logo=microsoftazure&logoColor=white)](https://azure.microsoft.com/)
[![Google Cloud](https://img.shields.io/badge/GoogleCloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white)](https://cloud.google.com/)
[![Terraform](https://img.shields.io/badge/terraform-%235835CC.svg?style=for-the-badge&logo=terraform&logoColor=white)](https://www.terraform.io/)
[![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)](https://kubernetes.io/)
[![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![OpenAI](https://img.shields.io/badge/OpenAI-%23412991.svg?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com/)

</div>

## 📋 Sobre o Projeto

CloudMart é uma plataforma de e-commerce completa para venda de produtos variados, desenvolvida com uma arquitetura moderna e escalável em nuvem. O projeto implementa funcionalidades essenciais de comércio eletrônico, incluindo:

- Catálogo de produtos diversificados
- Painel de administração robusto
- Sistema de pedidos integrado
- Suporte ao cliente com inteligência artificial
- Infraestrutura totalmente em nuvem

## 🌟 Funcionalidades Principais

- **Catálogo de produtos**: Exposição de produtos variados com descrições, imagens e preços
- **Carrinho de compras**: Sistema intuitivo para seleção e finalização de pedidos
- **Painel administrativo**: Interface completa para gestão de produtos, estoque e pedidos
- **Análise de dados**: Insights sobre vendas e comportamento dos clientes

## 🏗️ Arquitetura e Tecnologias

O CloudMart foi implementado com uma arquitetura moderna baseada em  multi-cloud:

### Infraestrutura 
- **Terraform**: Infraestrutura como código para provisionamento automatizado
- **AWS**: Serviços principais de hospedagem e computação
- **Docker**: Containerização de todos os componentes da aplicação
- **Kubernetes**: Orquestração de containers para escalabilidade e resiliência

### Implementações Principais
- ➡️ Provisionamento de tabelas SQL-DynamoDB pelo Terraform e Dockerização via AWS-EC2
- ➡️ Orquestração de containers Docker utilizando Kubernetes via AWS-EC2
- ➡️ AWS Pipeline - CI/CD para integração e entrega contínuas
- ➡️ Agentes de IA utilizando AWS-Bedrock e OpenIA para suporte ao cliente
- ➡️ BigQuery utilizando Google Cloud e análise de atendimento utilizando Azure Cloud

### Backend
- Banco de dados: DynamoDB (AWS)
- Node.JS
- Express.JS

### Frontend
- HTML
- Tailwind CSS
- JavaScript
- React.JS

## 🚀 Como Executar

### Pré-requisitos
- Conta AWS
- Conta Azure
- Conta Google Cloud
- Docker instalado
- Terraform instalado
- kubectl configurado
- Node instalado

### Instalação e Configuração

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/cloudmart.git
cd cloudmart
```

2. Configure as credenciais de nuvem:
```bash
# Configure AWS CLI
aws configure

# Configure outras credenciais conforme necessário
```

3. Execute o Terraform para provisionar a infraestrutura:
```bash
cd terraform
terraform init
terraform apply
```

4. Deploy da aplicação via Kubernetes:
```bash
kubectl apply -f kubernetes/
```

## 📊 Diagrama de Arquitetura

```
+------------------+     +------------------+     +------------------+
|                  |     |                  |     |                  |
|   AWS Services   |     |  Azure Services  |     |  Google Cloud    |
|   - EC2          |     |  - Azure AI      |     |  - BigQuery      |
|   - DynamoDB     |     |  - Analysis      |     |  - GKE           |
|   - Bedrock      |     |                  |     |                  |
+--------+---------+     +--------+---------+     +--------+---------+
         |                        |                        |
         v                        v                        v
+--------------------------------------------------+
|                                                  |
|              Kubernetes Cluster                  |
|     +----------------+    +----------------+     |
|     |                |    |                |     |
|     |  Frontend      |    |  Backend       |     |
|     |  Containers    |    |  Containers    |     |
|     |                |    |                |     |
|     +----------------+    +----------------+     |
|                                                  |
+--------------------------------------------------+
                      |
                      v
+--------------------------------------------------+
|                                                  |
|              CloudMart Application               |
|                                                  |
+--------------------------------------------------+
```

## 📧 Contato

Entre em contato através de [ryanluc.dev18@gmail.com](mailto:ryanluc.dev18@gmail.com)
