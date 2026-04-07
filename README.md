<div align="center">

# 🧠 Lista 1 — Lógica de Programação de Algoritmos

[![Status](https://img.shields.io/badge/status-concluído-brightgreen?style=flat-square)](.)
[![Curso](https://img.shields.io/badge/curso-Técnico%20em%20Dev.%20de%20Sistemas-blue?style=flat-square)](.)
[![Disciplina](https://img.shields.io/badge/disciplina-Lógica%20de%20Programação-purple?style=flat-square)](.)
[![Algoritmos](https://img.shields.io/badge/algoritmos-5-orange?style=flat-square)](.)

> *"Antes de escrever código, aprenda a pensar. A lógica é a base de tudo."*

</div>

---

## 📋 Sobre a Atividade

Esta é a **Lista 1 de Lógica de Programação**, desenvolvida como parte do **Curso Técnico em Desenvolvimento de Sistemas**. O objetivo é afastar o foco da sintaxe de linguagens de programação e exercitar o que realmente importa: **o raciocínio lógico e a decomposição de problemas**.

Para cada tarefa cotidiana foram elaborados:
- 📊 **Fluxograma** — representação visual do passo a passo com decisões e laços
- 📝 **Pseudocódigo** — descrição do algoritmo em linguagem próxima ao português estruturado

---

## 📚 Algoritmos Desenvolvidos

| # | Algoritmo | Estruturas Utilizadas |
|---|---|---|
| 1 | 🚶 [Ir ao Trabalho](#1-️-ir-ao-trabalho) | `SE/ENTÃO`, `ENQUANTO`, `LEIA`, `ESCREVA` |
| 2 | 🔧 [Troca de Pneu](#2--troca-de-pneu) | `SE/ENTÃO`, `PARE`, `LEIA`, `ESCREVA` |
| 3 | 💡 [Troca de Lâmpada](#3--troca-de-lâmpada) | `SE/ENTÃO`, `ENQUANTO`, `LEIA`, `ESCREVA` |
| 4 | 🚌 [Pegar um Ônibus](#4--pegar-um-ônibus) | `SE/ENTÃO`, `ENQUANTO`, `LEIA`, `ESCREVA` |
| 5 | 🎂 [Preparar um Bolo](#5--preparar-um-bolo-simples) | `ENQUANTO`, `variáveis`, `LEIA`, `ESCREVA` |

---

## 🔑 Conceitos-Chave

Antes de ver os algoritmos, é importante entender as estruturas utilizadas:

| Estrutura | Descrição | Quando usar |
|---|---|---|
| `SE / ENTÃO / SENÃO` | Executa um bloco de acordo com uma condição | Quando há uma decisão com dois caminhos possíveis |
| `ENQUANTO / FAÇA` | Repete um bloco enquanto a condição for verdadeira | Quando não sabemos quantas repetições serão necessárias |
| `LEIA` | Recebe um dado de entrada (do usuário ou do ambiente) | Para capturar informações externas |
| `ESCREVA` | Exibe uma saída ou executa uma ação | Para registrar cada passo do algoritmo |
| `PARE` | Interrompe o algoritmo antecipadamente | Quando uma condição impede a continuidade |

---

## 1. 🚶 Ir ao Trabalho

> **Problema:** Descrever o passo a passo para sair de casa e chegar ao trabalho — sem esquecer o crachá.

**Pontos de atenção:**
- 🔁 Laço obrigatório para garantir que o crachá seja encontrado antes de sair
- 🔀 Decisão sobre o meio de transporte (carro, ônibus ou a pé)
- ✅ Etapas não podem ser puladas (ex: sem abrir a porta não dá para sair)

### Fluxograma

```
┌─────────────┐
│    INÍCIO   │
└──────┬──────┘
       ↓
┌──────────────────────┐
│  Acordar e levantar  │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│   Higiene pessoal    │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│   Vestir roupa       │
└──────────┬───────────┘
           ↓
    ┌──────┴──────┐
    │ Está com o  │
    │   crachá?   │◄──────────┐
    └──────┬──────┘           │
     Sim ↓    └─ Não          │
           ↓         ┌────────┴────────┐
┌──────────────────────┐  │ Procurar o crachá │
│   Tomar café         │  └─────────────────┘
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│  Abrir porta e sair  │
└──────────┬───────────┘
           ↓
    ┌──────┴──────────┐
    │  Meio de        │
    │  transporte?    │
    └──┬────┬─────┬───┘
  Carro↓  Ônibus↓  A pé↓
  [dirigir] [ponto] [caminhar]
       └──────┴───────┘
                ↓
┌──────────────────────┐
│  Passar o crachá na  │
│      catraca         │
└──────────┬───────────┘
           ↓
┌─────────────┐
│     FIM     │
└─────────────┘
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

## 2. 🔧 Troca de Pneu

> **Problema:** Descrever com segurança o processo de trocar um pneu furado na beira da estrada.

**Pontos de atenção:**
- ⚠️ Verificação do estepe **antes** de começar — se estiver ruim, o algoritmo para e chama assistência
- 🔩 Afrouxar parafusos **antes** de levantar o carro (detalhe crítico de segurança)
- ✅ Parafusos devem ser apertados em forma de cruz para distribuir a pressão

### Fluxograma

```
┌─────────────┐
│    INÍCIO   │
└──────┬──────┘
       ↓
┌──────────────────────┐
│  Acionar pisca-alerta │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Parar em local seguro │
└──────────┬───────────┘
           ↓
┌──────────────────────────┐
│ Pegar estepe e macaco    │
└──────────┬───────────────┘
           ↓
    ┌──────┴──────┐
    │  Estepe em  │
    │  boas cond? │
    └──┬──────────┘
  Sim ↓       └─ Não → [Chamar assistência] → FIM
       ↓
┌──────────────────────────┐
│ Afrouxar parafusos (parcial)│
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│  Posicionar o macaco     │
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│    Elevar o carro        │
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│ Remover pneu / colocar   │
│       estepe             │
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│ Abaixar e apertar em cruz│
└──────────┬───────────────┘
           ↓
┌─────────────┐
│     FIM     │
└─────────────┘
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

## 3. 💡 Troca de Lâmpada

> **Problema:** Substituir uma lâmpada queimada com segurança, usando escada se necessário.

**Pontos de atenção:**
- ⚡ Desligar o interruptor é a **primeira etapa obrigatória** (segurança elétrica)
- 🌡️ Aguardar esfriar evita queimaduras
- 🔁 Laço de verificação garante que a lâmpada nova é compatível antes de instalar

### Fluxograma

```
┌─────────────┐
│    INÍCIO   │
└──────┬──────┘
       ↓
┌──────────────────────────┐
│  Desligar o interruptor  │
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│   Aguardar esfriar 5min  │
└──────────┬───────────────┘
           ↓
    ┌──────┴──────┐
    │ Precisa de  │
    │   escada?   │
    └──┬──────────┘
  Não ↓       └─ Sim → [Buscar e posicionar escada]
       ↓                          ↓
       └──────────────────────────┘
                    ↓
┌──────────────────────────┐
│  Remover lâmpada queimada │
└──────────┬───────────────┘
           ↓
    ┌──────┴──────┐
    │  Lâmpada    │◄──────────────┐
    │ compatível? │               │
    └──┬──────────┘               │
  Sim ↓    └─ Não → [Buscar lâmpada correta] ──┘
       ↓
┌──────────────────────────┐
│   Instalar nova lâmpada  │
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│  Descer e ligar interrup.│
└──────────┬───────────────┘
           ↓
┌─────────────┐
│     FIM     │
└─────────────┘
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

## 4. 🚌 Pegar um Ônibus

> **Problema:** Descrever o processo de usar transporte público com cartão de integração, do planejamento ao desembarque.

**Pontos de atenção:**
- 💳 Verificação de saldo **antes** de ir ao ponto — evita transtornos
- 🔁 Laço de espera para o ônibus correto — nem todo ônibus que passa é o desejado
- 🔔 Acionar a campainha antes da parada desejada é etapa crítica

### Fluxograma

```
┌─────────────┐
│    INÍCIO   │
└──────┬──────┘
       ↓
┌──────────────────────────┐
│ Consultar linha/horário  │
└──────────┬───────────────┘
           ↓
    ┌──────┴──────┐
    │  Saldo ok?  │
    └──┬──────────┘
  Sim ↓       └─ Não → [Recarregar o cartão]
       ↓                         ↓
       └─────────────────────────┘
                    ↓
┌──────────────────────────┐
│   Ir ao ponto de ônibus  │
└──────────┬───────────────┘
           ↓
    ┌──────┴──────┐
    │  É o ônibus │◄──────────────┐
    │   correto?  │               │
    └──┬──────────┘               │
  Sim ↓    └─ Não → [Aguardar próximo] ──┘
       ↓
┌──────────────────────────┐
│  Aguardar parar + embarcar│
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│    Validar o cartão      │
└──────────┬───────────────┘
           ↓
    ┌──────┴──────┐
    │  Chegou ao  │◄──────────────┐
    │  destino?   │               │
    └──┬──────────┘               │
  Sim ↓    └─ Não → [Aguardar] ──┘
       ↓
┌──────────────────────────┐
│ Acionar campainha e sair │
└──────────┬───────────────┘
           ↓
┌─────────────┐
│     FIM     │
└─────────────┘
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

## 5. 🎂 Preparar um Bolo Simples

> **Problema:** Descrever o processo completo de fazer um bolo, desde verificar os ingredientes até o teste do palito.

**Pontos de atenção:**
- 🔥 Pré-aquecer o forno é etapa **obrigatória antes** de preparar a massa
- 🥄 O fermento deve ser adicionado por último e misturado levemente
- 🔁 O teste do palito é uma condição de saída do laço — o bolo só sai do forno quando estiver pronto

### Fluxograma

```
┌─────────────┐
│    INÍCIO   │
└──────┬──────┘
       ↓
┌──────────────────────────────┐
│   Listar ingredientes        │
│ (ovos, farinha, açúcar, etc) │
└──────────┬───────────────────┘
           ↓
    ┌──────┴──────┐
    │  Todos ing. │◄──────────────┐
    │ disponíveis?│               │
    └──┬──────────┘               │
  Sim ↓    └─ Não → [Comprar faltantes] ─┘
       ↓
┌──────────────────────────┐
│  Pré-aquecer forno 180°C │
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│   Preparar a massa       │
│  (misturar ingredientes) │
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│  Untar forma + despejar  │
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│   Levar ao forno 40min   │
└──────────┬───────────────┘
           ↓
    ┌──────┴──────┐
    │   Palito    │◄──────────────┐
    │  sai limpo? │               │
    └──┬──────────┘               │
  Sim ↓    └─ Não → [+10 minutos] ┘
       ↓
┌──────────────────────────┐
│  Retirar e aguardar      │
│       esfriar            │
└──────────┬───────────────┘
           ↓
┌─────────────┐
│     FIM     │
└─────────────┘
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

## 🧩 O que Aprendemos com Estes Algoritmos?

### A regra de ouro da lógica de programação

> **Se você não mandar "abrir a porta", não tem como "sair de casa"!** 🚪

Cada algoritmo nesta lista reforça princípios fundamentais:

**1. Decomposição de problemas**
Todo problema complexo pode ser quebrado em passos simples e sequenciais. Trocar um pneu parece difícil, mas vira trivial quando você lista cada etapa com clareza.

**2. Decisões (estruturas condicionais)**
O mundo real é cheio de bifurcações. O algoritmo precisa prever todos os caminhos possíveis — e o que fazer em cada um deles.

**3. Repetição (estruturas de laço)**
Algumas etapas precisam ser feitas várias vezes até uma condição ser satisfeita. O palito no bolo só sai quando a massa estiver assada — não importa quantas tentativas.

**4. Validação antes de agir**
Verificar o saldo antes de ir ao ponto, checar o estepe antes de começar a troca — a lógica de programação nos ensina a **sempre validar antes de executar**.

---

## 📁 Estrutura do Repositório

```
📦 lista1-logica-algoritmos
 ┣ 📄 README.md          ← você está aqui
 ┗ 📄 algoritmos.md      ← pseudocódigos detalhados
```

---

## 👨‍💻 Informações

| Campo | Detalhe |
|---|---|
| 📚 Disciplina | Lógica de Programação |
| 🏫 Curso | Técnico em Desenvolvimento de Sistemas |
| 📋 Atividade | Lista 1 — Algoritmos do Cotidiano |
| 🛠️ Ferramentas | Pseudocódigo + Fluxograma |

---

<div align="center">

*Feito com 🧠 lógica e ☕ café*

</div>
