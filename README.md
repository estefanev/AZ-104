💻 Projeto Azure – Criação e Gerenciamento de Máquinas Virtuais

## 📘 Descrição Geral

Este repositório documenta a criação, configuração, gerenciamento e alterações realizadas em uma máquina virtual (VM) no Microsoft Azure. A atividade foi desenvolvida com o objetivo de consolidar conhecimentos práticos sobre infraestrutura em nuvem, gerenciamento de recursos e documentação técnica.

O projeto inclui a criação de uma VM com base no Windows Server 2019, alteração de seu tamanho e disco, desanexação de disco adicional, bem como a estruturação da rede virtual. Toda a configuração foi feita por meio do portal web do Azure, utilizando uma conta de estudante da plataforma.

---

## 🎯 Objetivos de Aprendizagem

- ✅ Aplicar os conceitos de infraestrutura como serviço (IaaS) na prática com o Azure.
- ✅ Documentar procedimentos técnicos de forma clara e padronizada.
- ✅ Utilizar o GitHub como repositório de conhecimento e versionamento de documentação técnica.

---

## 🧪 Tecnologias e Ferramentas Utilizadas

| Tecnologia      | Descrição                             |
|------------------|-----------------------------------------|
| **Microsoft Azure** | Plataforma de computação em nuvem utilizada para a criação e gerenciamento de recursos |
| **Windows Server 2019** | Imagem base da máquina virtual criada |
| **GitHub**       | Plataforma para hospedagem da documentação técnica |
| **Markdown**     | Linguagem de marcação utilizada no `README.md` |

---

## 🛠️ Etapas Realizadas

### 🏗️ 1. Criação da Máquina Virtual
- **Nome**: AZ-104-VM-1
- **Imagem**: Windows Server 2019 Datacenter – Gen2
- **Arquitetura**: x64
- **Região**: West US 3
- **Tipo de segurança**: Inicialização confiável com Secure Boot e vTPM ativados
- **Grupo de recursos**: `AZ-104`
- **Tamanho Inicial**: Standard D2s v3 (2 vCPUs, 8 GiB de memória)
- **Licença do Windows**: Nova licença vinculada ao Azure

---

### 🔁 2. Alterações Realizadas

- ✅ **Alteração do tamanho da VM** para otimização de custo/performance.
- ✅ **Alteração do disco** para SSD Premium (LRS).
- ✅ **Desanexação de disco adicional** configurado após testes iniciais.
- ✅ **Configuração de rede virtual (VNet)** com sub-rede padrão (`10.0.0.0/24`).
- ✅ **Ativação de portas públicas HTTP** para acesso externo.
- ❌ Monitoramento e diagnósticos foram **desativados** por estratégia de simplicidade no cenário atual.

---

## 🌐 Configurações de Rede

- **Rede virtual**: `AZ-104-VM-1-vnet`
- **Sub-rede**: `default (10.0.0.0/24)`
- **IP Público**: Ativado (dinâmico)
- **Grupo de Segurança de Rede (NSG)**: Regras básicas com porta 80 (HTTP)
- **Rede acelerada**: Desativada
- **Exclusão de recursos vinculados (IP/NIC)** ao deletar VM: Ativada

---

## 🧩 Recursos Associados

| Tipo de Recurso     | Nome                    |
|---------------------|-------------------------|
| Máquina Virtual     | AZ-104-VM-1, AZ-104-VM-2 |
| IP Público          | AZ-104-VM-1-ip, AZ-104-VM-2-ip |
| Rede Virtual        | AZ-104-VM-1-vnet         |
| Sub-rede            | default (10.0.0.0/24)    |
| Disco do SO         | SSD Premium (LRS)        |

---

## 🖼️ Documento em WORD

[📄 criacaivm-104.docx](./criacaivm-104.docx)

---

## 📂 Estrutura do Repositório

```bash
azure-vm-projeto/
├── README.md
└── images/
    ├── criacao-vm.png
    ├── alteracao-disco.png
    ├── desanexar-disco.png
    └── rede-configurada.png
```

---

## 📌 Considerações Finais

Este projeto demonstrou a criação e gerenciamento de uma máquina virtual no Azure com foco na documentação e boas práticas em nuvem. Ele reforça conceitos como provisionamento de recursos, controle de custos, segurança e organização de rede, aliados a uma documentação técnica eficaz.

---

## 🔗 Link do Projeto

🔗 **[Repositório GitHub](https://github.com/estefanev/AZ-104.git)**  


---

## 👨‍🎓 Autor

- **Nome:** Estefane Vieira
- **Curso:** Microsoft - Azure Administrator Certification (AZ-104)  
