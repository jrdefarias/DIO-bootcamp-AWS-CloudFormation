# ☁️ Implementando minha Primeira Stack com AWS CloudFormation

## 📚 Sobre o desafio

Este projeto foi desenvolvido como parte do desafio da plataforma DIO com foco em introdução ao AWS CloudFormation.

O objetivo foi entender na prática como funciona a criação de infraestrutura na nuvem utilizando arquivos de configuração automatizados, facilitando o gerenciamento e padronização de recursos na AWS.

Durante o laboratório consegui aprender conceitos importantes sobre Infraestrutura como Código IaC (Infrastructure as Code) e como a AWS permite automatizar processos através do CloudFormation.

---

# 🚀 O que é AWS CloudFormation?

O AWS CloudFormation é um serviço da AWS que permite criar e gerenciar recursos da nuvem através de arquivos em formato YAML ou JSON.

Ao invés de criar tudo manualmente pelo console da AWS, podemos definir a infraestrutura em um template e deixar que a AWS faça toda a criação automaticamente.

Isso ajuda em:

- Padronização de ambientes
- Automação de infraestrutura
- Redução de erros manuais
- Facilidade para recriar ambientes
- Controle de versão usando GitHub

---

# 📖 Conceitos aprendidos

## 📌 Stack

Uma Stack é um conjunto de recursos criados e gerenciados pelo CloudFormation.

**Exemplo de recursos que podem ser agrupados em uma única Stack:**
- EC2
- Security Groups
- Buckets S3
- Redes VPC

Todos estes recursos podem ser agrupados dentro de uma Stack.

---

## 📌 Template YAML

O template é o arquivo responsável por descrever toda a infraestrutura.

Exemplo simples:

```yaml
Resources:
  # Criação do bucket S3
  S3Bucket:
    Type: 'AWS::S3::Bucket'
    Properties:
      BucketName: s3-lab-cloudformation
```

Com isso o CloudFormation entende que deve criar um Bucket S3.

---

# ✅ Conclusão

Este desafio foi importante para entender os primeiros passos com AWS CloudFormation e Infraestrutura como Código.

Com certeza foi uma experiência muito válida para continuar evoluindo nos estudos de Cloud Computing e automação de infraestrutura.

---

# 🔗 Links úteis

- [Documentação AWS CloudFormation](https://docs.aws.amazon.com/pt_br/cloudformation/)
