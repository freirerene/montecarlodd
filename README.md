# Monte Carlo

Usamos simulação de Monte Carlo para estimar o drawdown médio e máximo (definido como o dd que ocorre 5% dos casos) para uma estratégia.

Da série histórica, que está no arquivo returns.csv extraímos a taxa de acerto (winrate) e a razão retorno:risco (rr). Usaremos apenas essas duas informações na simulação.

Na simulação: sorteamos números (pseudo)aleatórios entre 0 e 1; se for menor que winrate consideramos um ganho em uma unidade (+1); caso contrário, temos a perda de uma unidade (-1).
