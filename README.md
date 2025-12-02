# LANL-Earthquake-Prediction

🔧 Funcionamento
- Upload do arquivo no Google Colab
- Rodar o código da maneira que está (com os arquivos na nuvem da AWS), ou baixar os arquivos e subir para o Google Drive e aplicar os paths do Google Drive no algoritmo.

📊 Algoritmo Principal
Random Forest Regressor com as seguintes configurações:
- 100 árvores de decisão
- Profundidade máxima: 15
- Divisão 80/20 treino/validação
- Treinamento: 200 segmentos, 20 features, 150000 amostras

🎯 Métricas de Performance
- MAE (Mean Absolute Error): Erro médio em segundos
- Feature Importance: Importância de cada característica
- Visualizações: Gráficos de análise

📈 Resultados
- O modelo alcançou um MAE de aproximadamente 0.9966 segundos na validação, demonstrando boa capacidade de previsão.

📋 Features Extraídas
| Categoria | Features | Descrição |
|-----------|----------|-----------|
| **Estatísticas** | `mean`, `std`, `min`, `max` | Medidas básicas do sinal |
| **Forma** | `skewness`, `kurtosis` | Assimetria e curtose da distribuição |
| **Energia** | `abs_energy`, `abs_mean` | Potência e energia do sinal |
| **Sísmicas** | `zero_crossing_rate`, `mean_abs_diff` | Características específicas para terremotos |

🚀 Aplicações
- Sistemas de alerta precoce para terremotos
- Monitoramento sísmico em tempo real
- Estudo de mecânica de falhas geológicas

📚 Referências
- Kaggle: LANL Earthquake Prediction (https://www.kaggle.com/c/LANL-Earthquake-Prediction)
