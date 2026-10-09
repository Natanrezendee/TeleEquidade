# Fine-Tuning do Llama 3.1 8B para Regulação Assistencial (SISREG)

Este repositório contém o código, os dados sintéticos e a metodologia para o ajuste fino do modelo **Meta-Llama-3.1-8B-Instruct** utilizando **QLoRA (4-bit)** e a biblioteca **Unsloth**.

## 📌 Descrição do Projeto
O objetivo deste trabalho é validar a viabilidade técnica de modelos de linguagem abertos de pequeno porte (*Small Language Models*) na classificação automática de prioridade assistencial (ALTA, MÉDIA, BAIXA) no âmbito da regulação em saúde pública.

## 📁 Estrutura do Repositório
- `data/`: Conjuntos de dados sintéticos de treinamento (15 e 45 casos) e testes às cegas (Conjunto 1 e Teste Adversarial em formato JSON e CSV).
- `FineTuning.py`: Notebook completo em Python/Colab para reprodução dos experimentos EXP-001, EXP-002 e EXP-003.

## 🛠️ Tecnologias Utilizadas
- **Modelo Base:** Meta-Llama-3.1-8B-Instruct
- **Ajuste Fino:** QLoRA (r=16, alpha=16) via Unsloth
- **Hardware Utilizado:** GPU NVIDIA T4 (Google Colab)
- **Formato de Saída:** Estruturado em JSON (`prioridade`)

## Autores
- Isaac Emanuel Pires de Almeida
- Natan Rezende Kiffer Magalhães
