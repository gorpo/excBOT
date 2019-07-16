# excBOT
Atualmente o BOT est� na vers�o v0.1.5(TESTE) e sua fun��o � automatizar arbitragens entre as EXC CRIPTO e BLEUTRADE. Sua estrat�gia principal � comprar mais barato e vender mais caro conforme SPREAD configurado pelo usu�rio.


# FUN��ES
* Monitorar livro de ordens
* Analisa e compara valores
* Analisa quantidades para definir compra
* Efetua compra, transfer�ncia e venda
* Mostrar saldo via Telegram
* Mostrar informa��es da arbitragem via Telegram
* Compra de valores m�nimos se saldo for insuficiente
* Auto balance
* Tratamento de erros response
* Calcula SPREAD
* Calcula FEE
* Simulador de arbitragem


# ATEN��O:
O BOT est� em fase de testes, N�O H� NENHUMA GARANTIA DE GANHOS. O BOT est� sendo desenvolvido, est� sujeito a erros e por esse motivo est� em constantes atualiza��es. O desenvolvedor do excBOT N�O SE RESPONSABILIZA POR PREJU�ZOS ocasionados por mal uso do BOT.

DICA:
* A principal configura��o do BOT para ficar positivo, � o SPREAD. No arquivo de configura��o, config.py, tem uma op��o para configura-lo.
* Para ficar positivo � necess�rio configurar o SPREAD + FEE.
* FEE  0.25 (EXC/BLEU)
* Configurar o spread correto para n�o ficar negativo por causa da FEE.

Spread refere-se � diferen�a entre o pre�o de compra (procura) e venda (oferta) de um ativo.

# COMO FUNCIONA
O BOT monitora os books e compara os valores, caso encontre oportunidades, compra mais barato em uma exchange e vender mais caro na outra e automaticamente executa os comandos em alguns segundos.

# COMO EXECUTAR
Ap�s instala��o e configura��o. Abra um terminal e execute o comando para que o BOT inicie o trabalho.

# INSTALA��O
1. Cadastre na EXC CRIPTO(https://exccripto.com) e BLEUTRADE(https://bleutrade.com)
2. Gerar Key/Secret na EXC e BLEU
3. Instalar python, pip e requests
4. Configurar BOT com KEYs (EXC e BLEU)
5. Rodar

#ATUALIZA��ES
VERS�O: 0.1.5
- Melhora no tratamento dos erros (RESPONSE)
- Adicionado informa��o sobre FEE
- Adicionado informa��o sobre Arbitragem
- Adicionado informa��o sobre SPREAD (em % e USDT)
- Adicionado simulador de arbitragem (Ajuda escolher melhor SPREAD)
- Corre��o ordens venda m�nima (Muita ordens abertas no book)
 - Melhora da fun��o AUTO BALANCE

VERS�O: 0.1.4
- Adicionado verifica��o de saldo
- Fun��o que informa se houve lucros ou perdas

VERS�O: 0.1.3
- Adicionado Mercado USDT (excbleu BTC/USDT)
- Adicionado informa��o do lucro nas arbitragens
- Formata��o logs telegram
- Formata��o logs txt

VERS�O: 0.1.2
- Adicionado logs em txt
- Adicionado logs via Telegram 

VERS�O: 0.1.1
- Adicionado auto balance
- Adicionado compra m�nima

VERS�O: 0.1.0
- Adicionado ordem de compra
- Adicionado ordem de transfer�ncia via DIREC TRANSFER
- Adicionado ordem de venda

VERS�O: 0.0.1
- Busca informa��es nas exchanges EXC e BLEU
- Monitora book no mercado BTC
- Monitora book no mercado DOGE
- Compara valores de compra e venda nas exchanges EXC e BLEU
- Verifica se existe oportunidade de arbitragem entre as exchanges
