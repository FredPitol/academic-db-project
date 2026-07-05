<img width="1280" height="640" alt="image" src="https://github.com/user-attachments/assets/46254b83-d034-4ef0-984e-4a83fcb402c8" />
# Projeto de Banco de Dados para Setor de RH (Acadêmico)

![Status do Projeto](https://img.shields.io/badge/status-concluído-brightgreen?style=for-the-badge)
[![Licença](https://img.shields.io/github/license/FredPitol/academic-db-project?style=for-the-badge)](https://github.com/FredPitol/academic-db-project/blob/main/LICENSE)

> Projeto completo de análise, modelagem e implementação de um banco de dados relacional para o setor de Recursos Humanos. Desenvolvido como avaliação na disciplina de Banco de Dados I, o projeto aborda a correção de um modelo de dados falho e sua implementação funcional em PostgreSQL e MySQL.

<br>

## 📜 Visão Geral do Projeto

Este repositório documenta a jornada de reestruturação de um sistema de banco de dados para um departamento de RH fictício. O objetivo principal foi aplicar na prática os conceitos teóricos de modelagem de dados, normalização e linguagem SQL para criar um sistema robusto, íntegro e eficiente.

O processo de desenvolvimento foi dividido em três etapas fundamentais:
1.  **Análise Crítica:** Diagnóstico de um modelo lógico pré-existente para identificar falhas de projeto, como violações de formas normais, cardinalidade incorreta e falta de integridade referencial.
2.  **Modelagem de Dados:** Redesenho do modelo lógico para criar uma estrutura de dados coesa e normalizada, utilizando boas práticas de modelagem para garantir a qualidade e a manutenibilidade do banco.
3.  **Implementação e Povoamento:** Tradução do modelo lógico corrigido em código SQL, com scripts DDL (Data Definition Language) para a criação do esquema e scripts DML (Data Manipulation Language) para o povoamento com dados de exemplo.

---

## 💡 O Desafio: Do Modelo Falho à Solução Otimizada

O ponto de partida foi um desafio comum no mundo real: herdar um projeto com problemas. A capacidade de identificar e corrigir essas falhas foi o foco central do trabalho.

#### Modelo Lógico Original (Ponto de Partida)
O modelo inicial continha diversas inconsistências que, em um ambiente de produção, levariam a anomalias de dados e problemas de performance.

![Modelo lógico com erros](https://github.com/FredPitol/academic-db-project/blob/main/assets/hr.png)

#### Modelo Lógico Corrigido (Solução Proposta)
Após uma análise detalhada, o modelo foi reestruturado para alinhar-se às regras de negócio e às formas normais. As melhorias garantem a integridade dos dados, eliminam redundâncias e estabelecem relacionamentos claros entre as entidades.

![Modelo lógico corrigido](https://github.com/FredPitol/academic-db-project/blob/main/assets/projeto_logico_corrigido.png)

---

## 🛠️ Tecnologias e Ferramentas

| Categoria | Tecnologia/Ferramenta |
| :--- | :--- |
| **Bancos de Dados** | PostgreSQL, MariaDB / MySQL |
| **Linguagem** | SQL (DDL, DML) |
| **Ferramenta de Modelagem**| Oracle SQL Developer Data Modeler |
| **Cliente SQL** | DBeaver |

---

## 🚀 Guia de Instalação e Uso

Para recriar o ambiente do projeto localmente, siga os passos abaixo.

### Pré-requisitos
* [Git](https://git-scm.com/) instalado.
* Um SGBD de sua escolha (PostgreSQL ou MySQL/MariaDB) instalado e em execução.

### 1. Clonar o Repositório
Abra seu terminal e execute o seguinte comando:
```bash
git clone [https://github.com/FredPitol/academic-db-project.git](https://github.com/FredPitol/academic-db-project.git)
cd academic-db-project
```

### 2. Executar os Scripts SQL
Os scripts foram separados para facilitar a manutenção. **Execute-os na ordem numérica.**

* **`01_schema_*.sql`**: Cria toda a estrutura de tabelas, chaves e relacionamentos.
* **`02_data_*.sql`**: Popula as tabelas com dados de amostra.

Escolha o diretório correspondente ao seu SGBD (`/sql/postgresql` ou `/sql/mysql`) e utilize um cliente SQL para executar os arquivos.

**Exemplo de execução para PostgreSQL via terminal (`psql`):**
```bash
# Conecte-se ao seu SGBD e crie um banco de dados chamado "uvv" antes de prosseguir.
# Em seguida, execute os scripts:
psql -U seu_usuario -d uvv -f sql/postgresql/01_schema_postgresql.sql
psql -U seu_usuario -d uvv -f sql/postgresql/02_data_postgresql.sql
```

Após a execução, o banco de dados estará completamente configurado e pronto para ser consultado.

---

## 👨‍💻 Autor

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/frederico-pitol/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/FredPitol)

*Este projeto foi desenvolvido para fins acadêmicos sob a orientação do Prof. Abrantes Araújo Silva Filho, na Universidade Vila Velha (UVV) em 26 de Junho de 2025.*
