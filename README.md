# 🚀 1. PBL MLOps Hands-On Lab: Governança, Tracking e Ciclo de Vida do Modelo

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python)
![MLflow](https://img.shields.io/badge/MLflow-Tracking%20%26%20Registry-0185CA?style=for-the-badge&logo=mlflow)
![Metodologia](https://img.shields.io/badge/Metodologia-PBL%20(Challenge--Based)-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen?style=for-the-badge)

# 📌 2. Desafio & Metodologia (PBL)

Em projetos tradicionais de Ciência de Dados, o foco costuma terminar no treinamento do algoritmo (métricas em um Jupyter Notebook). 
No entanto, modelos isolados não geram valor sustentável em produção se não houver rastreabilidade, reprodutibilidade e automação.

Ao adotar a metodologia **Project-Based Learning (PBL)**, este lab foi construído para resolver um problema real: 

**Como migrar de um script de Machine Learning puro para uma esteira governada e auditável de MLOps?**

---

# 🛠️ 3. Arquitetura da Solução: ML vs. MLOps

O projeto separa rigidamente a **construção do algoritmo** do **gerenciamento do ciclo de vida**:

```text
       ┌────────────────────────────────────────────────────────┐
       │             CAMADA DE MACHINE LEARNING                 │
       │   Ingestão de Dados  ──>  Treino  ──>  Avaliação       │
       └───────────────────────────┬────────────────────────────┘
                                   │
       ┌───────────────────────────▼────────────────────────────┐
       │             CAMADA DE MLOPS & GOVERNANÇA               │
       │ 1. Rastreio (Parâmetros, Métricas e Hiperparâmetros)   │
       │ 2. Validação Automatizada (Quality Gates)              │
       │ 3. Versionamento & Registro (MLflow Model Registry)    │
       │ 4. Promoção de Ambientes (Staging / Production)        │
       └────────────────────────────────────────────────────────┘
```
# 🛠️ 4. Competências Técnicas Demonstradas
Rastreamento de Experimentos (Experiment Tracking): Captura sistemática de parâmetros, versões de dados e métricas com MLflow.

Portões de Qualidade (Quality Gates): Validação automatizada antes da aprovação do artefato para impedir que modelos degradados entrem em registro.

Gestão de Artefatos & Model Registry: Registro e versionamento unívoco do binário do modelo .pkl.

Governança & Linhagem (Lineage): Mapeamento que conecta o commit do código ao dataset e ao modelo final promovido.

# 📊 5. Evidências do MLOps em Ação
(Insirir capturas de tela da interface visual do MLflow executando)

Rastreio de Experimentos (Metrics & Params)

Model Registry & Versionamento

# ⚙️ 6. Como Executar o Projeto

Pré-requisitos:

Python 3.10+

Git

6.1. Clonar o repositório
git clone [https://github.com/seu-usuario/pbl-mlops-hands-on-lab.git](https://github.com/seu-usuario/pbl-mlops-hands-on-lab.git)

cd pbl-mlops-hands-on-lab

6.2. Criar e ativar o ambiente virtual
python -m venv .venv

source .venv/bin/activate # Linux/macOS # .venv\Scripts\activate  # Windows

6.3. Instalar dependências

pip install -r requirements.txt

6.4. Executar a esteira de treino e MLOps

python src/train.py

6.5. Abrir o Dashboard do MLflow

mlflow ui

# 💡 7. Principais Aprendizados

Machine Learning cria o modelo; MLOps o sustenta.

A inclusão de um Quality Gate na esteira impede que artefatos com desempenho inferior ao baseline atinjam o repositório central.

A governança garante reprodutibilidade total em auditorias futuras.

# 👤 8. Autoria e Créditos

Este laboratório prático (PBL) foi idealizado e construído por mim, **Janaína Nascimento Feitoza**,
a partir dos fundamentos e práticas apresentados durante o **Workshop Online de MLOps**
promovido pelo **INDT (Instituto de Desenvolvimento Tecnológico)**,
adaptando a teoria para uma estrutura governada de aprendizado por projetos.

- **LinkedIn:** [https://www.linkedin.com/in/jana%C3%ADna-nascimento-feitoza-27559920a]

- **GitHub:** [https://github.com/jana-nf]
