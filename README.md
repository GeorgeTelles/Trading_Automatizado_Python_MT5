<img src="https://raw.githubusercontent.com/GeorgeTelles/georgetelles/f69531ec6b293b5148563588a764c010015d315e/logo_clara.png" width="300" align="left"/>
<img src="https://raw.githubusercontent.com/GeorgeTelles/georgetelles/f69531ec6b293b5148563588a764c010015d315e/logo_dark.png" width="300" align="left"/>


<br>
<br>

# **Algoritmo Automatizado de Trading com Python e MetaTrader5**
------

Este projeto implementa um algoritmo em Python que aplica uma estratégia de trading a múltiplos ativos financeiros simultaneamente, utilizando o MetaTrader5 para executar operações de compra automaticamente.

## Funcionalidades

1. **Instalação e Importação de Bibliotecas**
   - Utiliza a biblioteca `MetaTrader5` para comunicação com a plataforma de trading.
   - Importa outras bibliotecas necessárias para manipulação de dados e cálculos financeiros.

2. **Configuração Inicial**
   - Conecta ao MetaTrader5 e configura os ativos desejados para análise.
   - Verifica a disponibilidade dos ativos na plataforma.

3. **Criação do Screening de Ativos**
   - **Download de Dados**: Coleta dados históricos de cotações para cada ativo.
   - **Cálculo de Indicadores**: Adiciona Médias Móveis Simples (SMA) de 20 e 200 períodos aos dados dos ativos.
   - **Regras de Estratégia**: Define regras para identificar quais ativos atendem aos critérios da estratégia, como:
     - A SMA de 20 períodos deve ser maior que a SMA de 200 períodos.
     - O preço de fechamento deve estar acima da SMA de 20 períodos.

4. **Automatização de Trades**
   - Monitora os ativos periodicamente para verificar se atendem às condições da estratégia.
   - Executa automaticamente ordens de compra para os ativos que cumprem os critérios, utilizando o MetaTrader5.
   - Implementa controle para evitar múltiplas ordens para o mesmo ativo e ajusta o volume, stop loss e take profit das ordens.

## Requisitos

- MetaTrader5 instalado e configurado.
- Python 3.x.
- Bibliotecas: `MetaTrader5`, `pandas`, `numpy`, `pytz`, `mplfinance`, `plotly`.

Este algoritmo é ideal para traders que desejam automatizar a aplicação de estratégias de trading em múltiplos ativos, economizando tempo e potencialmente melhorando a eficiência das operações.
