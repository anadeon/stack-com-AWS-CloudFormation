# Desafio Módulo 8 – Santander Code Girls 💻☁️

Este repositório é referente ao **desafio do Módulo 8 do curso Santander: Code Girls**, cujo objetivo era apresentar um **resumo e anotações** feitas durante o módulo, com foco na **criação de stacks utilizando AWS CloudFormation**.


## ☁️ O que é AWS CloudFormation

O **AWS CloudFormation** é um serviço da AWS que permite **automatizar a criação e gerenciamento de recursos na nuvem** por meio de **templates escritos em JSON ou YAML**.

Você pode definir tudo em um único arquivo, como:
- Instâncias EC2
- Buckets S3
- Databases RDS
- E muito mais

### 🛠️ Vantagens:
- Reutilização de templates
- Automatização de infraestrutura
- Paga-se apenas pelos **recursos criados**, não pelo uso do CloudFormation em si


## 📦 Criando Stacks com AWS CloudFormation

Uma **stack** é um conjunto de recursos definidos em um template. Abaixo, um **exemplo simples** de como criar uma instância EC2 usando YAML.

### 🧾 Exemplo de template básico (EC2):

```yaml
AWSTemplateFormatVersion: "2010-09-09"
Description: "Criação simples de uma instância EC2"

Resources:
  MinhaInstanciaEC2:
    Type: "AWS::EC2::Instance"
    Properties:
      ImageId: "ami-0c55b159cbfafe1f0"  # Amazon Linux 2 (exemplo para us-east-1)
      InstanceType: "t2.micro"
```

### 📌 Como criar uma stack com esse template:

1. Acesse o serviço CloudFormation no Console da AWS

2. Clique em "Criar stack" → "Com novos recursos (padrão)"

3. Escolha a opção "Fazer upload de um arquivo de template"

4. Envie o arquivo .yaml com o conteúdo acima

5. Avance, dê um nome à stack (ex: MinhaStackEC2)

6. Clique em "Criar stack" e aguarde a finalização

### ✅ Conclusão


O AWS CloudFormation é uma excelente ferramenta para quem quer automatizar a criação de infraestrutura na nuvem, garantindo padronização, agilidade e controle de mudanças. Com poucos comandos, é possível provisionar ambientes inteiros de forma segura e repetível.

---
Feito por Ana Gabriela Deon ✨👩🏻‍💻
