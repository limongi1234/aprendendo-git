# Métricas de Classificação 📊

Script em **Python** que calcula as principais **métricas de avaliação de modelos de classificação** a partir dos valores de uma matriz de confusão (VP, VN, FP, FN).

## ✨ Métricas calculadas

A função `calcular_metricas(vp, vn, fp, fn)` retorna um dicionário com:

| Métrica | Fórmula |
|--------------------|------------------------------------------|
| **Acurácia** | (VP + VN) / (VP + VN + FP + FN) |
| **Sensibilidade** (recall) | VP / (VP + FN) |
| **Especificidade** | VN / (VN + FP) |
| **Precisão** | VP / (VP + FP) |
| **F-score** | 2 × (Precisão × Sensibilidade) / (Precisão + Sensibilidade) |

O script já inclui um **exemplo de uso** (VP=80, VN=70, FP=20, FN=30) que imprime cada métrica com 2 casas decimais.

## 🛠️ Tecnologias

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)

- **Python** puro (sem dependências externas)

## 🚀 Como executar

```bash
git clone https://github.com/limongi1234/Metricas.git
cd Metricas

# o arquivo principal é "CalculoMetricas" — renomeie para .py se preferir
python3 CalculoMetricas
```

Saída esperada (exemplo embutido):

```
acuracia: 0.75
sensibilidade: 0.73
especificidade: 0.78
precisao: 0.80
f_score: 0.76
```

> 💡 Dica: renomear o arquivo para `calculo_metricas.py` facilita importar a função em outros projetos: `from calculo_metricas import calcular_metricas`.

> 📚 Projeto de estudo sobre avaliação de modelos de Machine Learning.
