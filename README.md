# Lista 1 — Lógica de Programação de Algoritmos

**Curso Técnico em Desenvolvimento de Sistemas**

> Atividade: elaborar algoritmos completos com pseudocódigo e descrição do fluxograma para tarefas cotidianas.

---

## Sumário

1. [Ir ao Trabalho](#1-ir-ao-trabalho)
2. [Troca de Pneu](#2-troca-de-pneu)
3. [Troca de Lâmpada](#3-troca-de-lâmpada)
4. [Pegar um Ônibus](#4-pegar-um-ônibus)
5. [Preparar um Bolo Simples](#5-preparar-um-bolo-simples)

---

## 1. Ir ao Trabalho

### Descrição do Fluxograma

```
INÍCIO
  → Acordar e levantar
  → Higiene pessoal (banho, escova dentes)
  → Vestir roupa de trabalho
  → [DECISÃO] Está com o crachá?
      NÃO → Voltar e procurar o crachá → (repete até encontrar)
      SIM → Tomar café da manhã
  → Abrir a porta e sair de casa
  → [DECISÃO] Qual meio de transporte?
      Carro/moto → Entrar no veículo e dirigir
      Ônibus     → Andar até o ponto e embarcar
      A pé       → Caminhar até o trabalho
  → Chegar ao trabalho
  → Passar o crachá na catraca
FIM
```

### Pseudocódigo

```
ALGORITMO IrAoTrabalho
INÍCIO
  ESCREVA("Acordar e levantar da cama")
  ESCREVA("Tomar banho")
  ESCREVA("Escovar os dentes")
  ESCREVA("Vestir roupas de trabalho")

  ENQUANTO cracha_visivel = FALSO FAÇA
    ESCREVA("Procurar o crachá")
    LEIA(cracha_visivel)
  FIM_ENQUANTO

  ESCREVA("Tomar café da manhã")
  ESCREVA("Abrir a porta de casa")
  ESCREVA("Sair de casa e fechar a porta")

  LEIA(meio_transporte)

  SE meio_transporte = "carro" ENTÃO
    ESCREVA("Entrar no carro")
    ESCREVA("Dirigir até o trabalho")
  SENÃO SE meio_transporte = "ônibus" ENTÃO
    ESCREVA("Andar até o ponto de ônibus")
    ESCREVA("Embarcar no ônibus")
  SENÃO
    ESCREVA("Caminhar até o trabalho")
  FIM_SE

  ESCREVA("Chegar ao trabalho")
  ESCREVA("Passar o crachá na catraca")
FIM_ALGORITMO
```

---

## 2. Troca de Pneu

### Descrição do Fluxograma

```
INÍCIO
  → Acionar o pisca-alerta
  → Parar o carro em local seguro (acostamento)
  → Pegar o estepe e o macaco do porta-malas
  → [DECISÃO] O estepe está calibrado e em boas condições?
      NÃO → Chamar assistência técnica → FIM
      SIM → Afrouxar os parafusos (sem remover completamente)
  → Posicionar o macaco no ponto correto do chassi
  → Elevar o carro com o macaco
  → Remover completamente os parafusos
  → Retirar o pneu furado
  → Colocar o estepe
  → Apertar os parafusos parcialmente
  → Abaixar o macaco até o carro tocar o chão
  → Apertar os parafusos definitivamente (em cruz)
  → Guardar pneu furado e macaco no porta-malas
FIM
```

### Pseudocódigo

```
ALGORITMO TrocaDePneu
INÍCIO
  ESCREVA("Acionar o pisca-alerta")
  ESCREVA("Parar o carro em local seguro")
  ESCREVA("Retirar estepe e macaco do porta-malas")

  LEIA(estepe_calibrado)

  SE estepe_calibrado = FALSO ENTÃO
    ESCREVA("Chamar assistência técnica")
    PARE
  FIM_SE

  ESCREVA("Afrouxar os parafusos sem remover")
  ESCREVA("Posicionar o macaco no chassi")
  ESCREVA("Elevar o carro com o macaco")
  ESCREVA("Remover completamente os parafusos")
  ESCREVA("Retirar o pneu furado")
  ESCREVA("Colocar o estepe no lugar")
  ESCREVA("Apertar os parafusos parcialmente")
  ESCREVA("Abaixar o macaco até o carro tocar o chão")
  ESCREVA("Apertar os parafusos definitivamente em cruz")
  ESCREVA("Guardar pneu furado e macaco no porta-malas")
FIM_ALGORITMO
```

---

## 3. Troca de Lâmpada

### Descrição do Fluxograma

```
INÍCIO
  → Desligar o interruptor
  → Aguardar a lâmpada esfriar (~5 minutos)
  → [DECISÃO] Alcança sem escada?
      NÃO → Buscar escada → Posicionar com segurança
      SIM → (continua)
  → Subir / aproximar-se da lâmpada
  → Girar a lâmpada para remover (sentido anti-horário)
  → [DECISÃO] A nova lâmpada é compatível (mesmo bocal/potência)?
      NÃO → Buscar lâmpada correta → (repete verificação)
      SIM → Instalar a nova lâmpada (sentido horário)
  → Descer da escada
  → Ligar o interruptor
  → [DECISÃO] A lâmpada acendeu?
      NÃO → Verificar circuito elétrico
      SIM → Concluído
FIM
```

### Pseudocódigo

```
ALGORITMO TrocaDeLampada
INÍCIO
  ESCREVA("Desligar o interruptor")
  ESCREVA("Aguardar 5 minutos para a lâmpada esfriar")

  LEIA(precisa_escada)

  SE precisa_escada = VERDADEIRO ENTÃO
    ESCREVA("Buscar a escada")
    ESCREVA("Posicionar a escada com segurança")
  FIM_SE

  ESCREVA("Subir / aproximar-se da lâmpada")
  ESCREVA("Girar a lâmpada no sentido anti-horário para remover")

  nova_lampada_ok <- FALSO

  ENQUANTO nova_lampada_ok = FALSO FAÇA
    ESCREVA("Verificar se a nova lâmpada é compatível")
    LEIA(nova_lampada_ok)
    SE nova_lampada_ok = FALSO ENTÃO
      ESCREVA("Buscar lâmpada com bocal e potência corretos")
    FIM_SE
  FIM_ENQUANTO

  ESCREVA("Instalar a nova lâmpada (sentido horário)")
  ESCREVA("Descer da escada")
  ESCREVA("Ligar o interruptor")

  LEIA(lampada_acendeu)

  SE lampada_acendeu = FALSO ENTÃO
    ESCREVA("Verificar o circuito elétrico ou chamar eletricista")
  FIM_SE
FIM_ALGORITMO
```

---

## 4. Pegar um Ônibus

### Descrição do Fluxograma

```
INÍCIO
  → Consultar o número da linha e horário desejado
  → [DECISÃO] Saldo no cartão é suficiente para a tarifa?
      NÃO → Recarregar o cartão de transporte
      SIM → (continua)
  → Deslocar-se até o ponto de ônibus
  → [DECISÃO] O ônibus que chegou é o da linha correta?
      NÃO → Aguardar o próximo ônibus → (repete verificação)
      SIM → Aguardar o ônibus parar completamente
  → Embarcar pela porta dianteira
  → Aproximar o cartão da catraca para validar
  → Encontrar assento ou local para ficar
  → [DECISÃO] Chegou ao destino?
      NÃO → Continuar aguardando → (repete)
      SIM → Acionar a campainha
  → Desembarcar pela porta traseira
FIM
```

### Pseudocódigo

```
ALGORITMO PegarOnibus
INÍCIO
  LEIA(numero_linha, horario_desejado)
  ESCREVA("Consultar horário da linha " + numero_linha)

  LEIA(saldo_cartao)
  LEIA(tarifa)

  SE saldo_cartao < tarifa ENTÃO
    ESCREVA("Recarregar o cartão de transporte")
  FIM_SE

  ESCREVA("Deslocar-se até o ponto de ônibus")

  onibus_correto <- FALSO

  ENQUANTO onibus_correto = FALSO FAÇA
    LEIA(onibus_chegou, numero_onibus)
    SE onibus_chegou = VERDADEIRO ENTÃO
      SE numero_onibus = numero_linha ENTÃO
        onibus_correto <- VERDADEIRO
      SENÃO
        ESCREVA("Aguardar próximo ônibus")
      FIM_SE
    FIM_SE
  FIM_ENQUANTO

  ESCREVA("Aguardar o ônibus parar completamente")
  ESCREVA("Embarcar pela porta dianteira")
  ESCREVA("Aproximar cartão da catraca para validar")
  ESCREVA("Encontrar assento ou local para ficar de pé")

  destino_alcancado <- FALSO

  ENQUANTO destino_alcancado = FALSO FAÇA
    ESCREVA("Observar as paradas do trajeto")
    LEIA(destino_alcancado)
  FIM_ENQUANTO

  ESCREVA("Acionar a campainha para desembarque")
  ESCREVA("Desembarcar pela porta traseira")
FIM_ALGORITMO
```

---

## 5. Preparar um Bolo Simples

### Descrição do Fluxograma

```
INÍCIO
  → Listar os ingredientes necessários
     (ovos, farinha, açúcar, óleo, leite, fermento)
  → [DECISÃO] Todos os ingredientes estão disponíveis?
      NÃO → Comprar ingredientes faltantes → (repete verificação)
      SIM → Pré-aquecer o forno a 180°C
  → Medir e separar todos os ingredientes
  → Bater os ovos com o açúcar e o óleo
  → Adicionar o leite e misturar
  → Peneirar e adicionar a farinha aos poucos
  → Adicionar o fermento por último (misturar levemente)
  → Untar e enfarinhar a forma
  → Despejar a massa na forma
  → Levar ao forno por 40 minutos
  → [DECISÃO] Palito inserido no centro sai limpo?
      NÃO → Assar por mais 10 minutos → (repete verificação)
      SIM → Retirar o bolo do forno
  → Aguardar esfriar antes de desenformar
FIM
```

### Pseudocódigo

```
ALGORITMO PrepararBolo
INÍCIO
  // Ingredientes: ovos, farinha, açúcar, óleo, leite, fermento

  ingredientes_disponiveis <- FALSO

  ENQUANTO ingredientes_disponiveis = FALSO FAÇA
    ESCREVA("Verificar ingredientes disponíveis")
    LEIA(ingredientes_disponiveis)
    SE ingredientes_disponiveis = FALSO ENTÃO
      ESCREVA("Comprar ingredientes faltantes")
    FIM_SE
  FIM_ENQUANTO

  ESCREVA("Pré-aquecer o forno a 180°C")
  ESCREVA("Medir e separar todos os ingredientes")

  // Preparar a massa
  ESCREVA("Bater os ovos com o açúcar e o óleo")
  ESCREVA("Adicionar o leite e misturar")
  ESCREVA("Peneirar e adicionar a farinha aos poucos")
  ESCREVA("Adicionar o fermento por último (misturar levemente)")

  ESCREVA("Untar e enfarinhar a forma")
  ESCREVA("Despejar a massa na forma")
  ESCREVA("Levar ao forno — tempo inicial: 40 minutos")

  tempo <- 40
  palito_limpo <- FALSO

  ENQUANTO palito_limpo = FALSO FAÇA
    ESCREVA("Testar o palito no centro do bolo")
    LEIA(palito_limpo)
    SE palito_limpo = FALSO ENTÃO
      ESCREVA("Assar por mais 10 minutos")
      tempo <- tempo + 10
    FIM_SE
  FIM_ENQUANTO

  ESCREVA("Retirar o bolo do forno")
  ESCREVA("Aguardar esfriar antes de desenformar")
  ESCREVA("Bolo concluído em " + tempo + " minutos!")
FIM_ALGORITMO
```

---

## Estruturas Utilizadas

| Estrutura | Utilização nos algoritmos |
|---|---|
| `SE / ENTÃO / SENÃO` | Decisões únicas: estepe ok?, lâmpada compatível?, saldo suficiente? |
| `ENQUANTO / FAÇA` | Repetição com condição: buscar crachá, aguardar ônibus certo, testar palito |
| `LEIA` | Entrada de dados do ambiente (resultado de ação, verificação) |
| `ESCREVA` | Saída / execução de um passo do algoritmo |
| `PARE` | Interrupção antecipada (ex: chamar assistência na troca de pneu) |

---

*Lista 1 — Lógica de Programação · Curso Técnico em Desenvolvimento de Sistemas*
