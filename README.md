# 🚀 SDW2025 – Pipeline ETL Portfólio

![GitHub Repo Size](https://img.shields.io/github/repo-size/your-username/SDW2025_Projeto_Portifolio)
![Python Version](https://img.shields.io/badge/Python-3.10+-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Ativo-success)

---

## 📘 Visão Geral

Este projeto apresenta um Pipeline **ETL (Extract – Transform – Load)** desenvolvido como parte do portfólio da **Santander Dev Week 2025 (SDW2025)**.

Com a indisponibilidade temporária da API oficial, uma solução alternativa robusta foi construída utilizando **Google Colab**, **GitHub como data host**, e integrações com a **API da OpenAI**.

O resultado é um fluxo completo de extração, transformação e carga de dados estruturados, totalmente funcional e documentado.

---

## 🧩 Tecnologias e Bibliotecas Utilizadas

Este projeto foi executado no Google Colab e requer a instalação das seguintes dependências:

```bash
!pip install cartopy
!apt-get -qq install -y graphviz && pip install pydot
!apt-get -qq install -y libarchive-dev && pip install -U libarchive
!apt-get -qq install -y libfluidsynth1
!pip install matplotlib-venn
!pip install openai
```

Essas ferramentas permitiram desde manipulação de dados até visualizações, leitura de arquivos compactados e integração com APIs externas.

---

## 🔄 Pipeline ETL

A seguir estão representadas as etapas que compõem o pipeline, junto das imagens correspondentes extraídas diretamente do ambiente do projeto.

### **📥 Extract**

Extração dos dados a partir de fontes públicas no GitHub e arquivos locais.


<img width="1382" height="865" alt="Extract" src="https://github.com/user-attachments/assets/dc358646-730b-49bc-b016-27cb72277ebe" />


---

### **🔧 Transform**

Processamento, padronização e enriquecimento dos dados, incluindo tentativas de integração via API da OpenAI.



---<img width="1617" height="494" alt="Transforms" src="https://github.com/user-attachments/assets/13ed5a6b-e706-4030-9e4b-8a0e8baa2f5b" />


<img width="1584" height="929" alt="Transforms - 2" src="https://github.com/user-attachments/assets/755d9a0a-0203-4fe8-9033-1ef4c3a55391" />


### **📤 Load**

Envio dos dados processados para endpoints simulados, replicando o conceito de atualização via API.


---<img width="1532" height="280" alt="Load" src="https://github.com/user-attachments/assets/6fec95ff-bf1b-4ea3-af6d-bd1877a8bbc2" />


## 📂 Estrutura do Projeto

```
SDW2025_Projeto_Portifólio/
│
├── dados.json               # Base completa dos usuários
├── SDW2025-userID.csv       # Lista de IDs dos usuários
├── README.md                # Documentação principal
└── exemplo_colab.ipynb      # Notebook ilustrando o pipeline
```

---

## 🧪 Detalhes Técnicos

### Criação da Base de Dados

Com a falta da API oficial, foi criada uma estrutura própria contendo:

* **usuarios.json** – Dados completos dos usuários.
* **SDW2025-userID.csv** – IDs usados como referência no pipeline.

Exemplo do conteúdo:

```
userID
4
5
6
```

### GitHub como API Estática

O GitHub foi utilizado como servidor de dados devido à sua disponibilidade e custo zero.

Vantagens:

* Alta confiabilidade
* Sem necessidade de backend
* Acesso público via URLs

### Uso da API OpenAI

O projeto envolveu tentativas de enriquecimento dos dados usando modelos da OpenAI. Porém, ocorreu o erro:

```
RateLimitError: 429 - You exceeded your current quota
```

O que impossibilitou a continuação da etapa em produção.

---

## 🧾 Conclusão

Apesar de limitações como cotas da API da OpenAI, o projeto demonstra domínio de:

* Arquitetura ETL
* Manipulação e enriquecimento de dados
* Uso do GitHub como fonte estática
* Execução completa via Google Colab

Este portfólio reflete capacidade técnica, adaptação a problemas reais e documentação para análise.

---

## 🙏 Agradecimentos

Este projeto é inspirado na jornada proporcionada pela **Digital Innovation One (DIO)**.

A toda a equipe, meu sincero agradecimento pelo conteúdo de qualidade, suporte contínuo e incentivo à prática.

Obrigado por construírem um ambiente acessível, acolhedor e transformador. Cada módulo, desafio e mentoria contribuiu diretamente para minha evolução.

💙 Este portfólio é um reflexo dessa trajetória.

---
