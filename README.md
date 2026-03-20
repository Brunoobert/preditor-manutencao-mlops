# 🚗 Nissan March Predictor: MLOps Lifecycle

Este projeto aplica os princípios de **MLOps (Machine Learning Operations)** para prever custos de manutenção preventiva do meu **Nissan March 2013**. O objetivo é transformar um modelo de regressão simples em um produto de software escalável, monitorado e automatizado.

---

## 🏗️ Arquitetura do Sistema

O projeto é dividido em quatro camadas principais, garantindo que o ciclo de vida do modelo seja completo:

1.  **Camada de Dados (Data Ops):** Gestão de datasets com `DVC` e armazenamento versionado.
2.  **Camada de Experimentos (ML):** Treinamento de modelos de regressão rastreados pelo `MLflow`.
3.  **Camada de Serventia (Serving):** Exposição do modelo via API `FastAPI` encapsulada em `Docker`.
4.  **Camada de Automação (CI/CD):** Pipeline automatizado via `GitHub Actions`.

---

## 🛠️ Stack Tecnológica

* **Linguagem:** Python 3.10+
* **Gestão de Dados:** DVC (Data Version Control)
* **Tracking:** MLflow (Métricas: $MAE$, $RMSE$)
* **Framework de ML:** Scikit-Learn
* **API:** FastAPI & Uvicorn
* **Infraestrutura:** Docker & Docker Compose
* **Ambiente:** WSL2 (Ubuntu) no Windows 11
* **CI/CD:** GitHub Actions

---

## 📋 Requisitos do Projeto

### Funcionais (RF)
* **RF01:** Rastrear versões de dados para evitar "Data Drift".
* **RF02:** Treinar modelo para prever custos baseados em quilometragem e idade.
* **RF03:** Registrar parâmetros e binários de modelos no MLflow.
* **RF04:** Fornecer interface de predição via endpoint HTTP.

### Não Funcionais (RNF)
* **RNF01:** Todos os serviços devem ser containerizados.
* **RNF02:** Garantir rastreabilidade total (Linagem de Dados).
* **RNF03:** Latência de predição inferior a 200ms.
* **RNF04:** Deploy automatizado após testes de integração.

---
## 📈 Status dos Milestones
[ ] Milestone 1: Setup de Infra (Docker + MLflow + DVC) - Em progresso

[ ] Milestone 2: Pipeline de Treinamento e Experimentos

[ ] Milestone 3: Criação da API e Containerização

[ ] Milestone 4: Automação CI/CD

[ ] Milestone 5: Monitoramento e Dashboard (Streamlit)

## 🚀 Como Executar (Em breve)
> *Nota: Instruções de execução serão adicionadas conforme a conclusão dos Milestones.*
>
```bash
# Exemplo de como subiremos o ambiente
docker-compose up -d



