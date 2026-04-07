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
- 📊 **Fluxograma** — representação visual do passo a passo
- 📝 **Pseudocódigo** — descrição do algoritmo em linguagem próxima ao português estruturado

---

## 📚 Algoritmos Desenvolvidos

| # | Algoritmo | Estruturas Utilizadas |
|---|---|---|
| 1 | 🚶 [Ir ao Trabalho](#1-️-ir-ao-trabalho) | `ENQUANTO`, `LEIA`, `ESCREVA` |
| 2 | 🔧 [Troca de Pneu](#2--troca-de-pneu) | `LEIA`, `ESCREVA` |
| 3 | 💡 [Troca de Lâmpada](#3--troca-de-lâmpada) | `ENQUANTO`, `LEIA`, `ESCREVA` |
| 4 | 🚌 [Pegar um Ônibus](#4--pegar-um-ônibus) | `ENQUANTO`, `LEIA`, `ESCREVA` |
| 5 | 🎂 [Preparar um Bolo](#5--preparar-um-bolo-simples) | `ENQUANTO`, `variáveis`, `LEIA`, `ESCREVA` |

---

## 🔑 Conceitos-Chave

Antes de ver os algoritmos, é importante entender as estruturas utilizadas:

| Estrutura | Descrição | Quando usar |
|---|---|---|
| `ENQUANTO / FAÇA` | Repete um bloco enquanto a condição for verdadeira | Quando não sabemos quantas repetições serão necessárias |
| `LEIA` | Recebe um dado de entrada (do usuário ou do ambiente) | Para capturar informações externas |
| `ESCREVA` | Exibe uma saída ou executa uma ação | Para registrar cada passo do algoritmo |

---

## 1. 🚶 Ir ao Trabalho

> **Problema:** Descrever o passo a passo para sair de casa e chegar ao trabalho — sem esquecer o crachá.

**Pontos de atenção:**
- 🔁 Laço obrigatório para garantir que o crachá seja encontrado antes de sair
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
┌──────────────────────┐
│  Procurar o crachá   │◄──┐
└──────────┬───────────┘   │
           ↓               │
┌──────────────────────┐   │
│  Crachá encontrado?  │───┘
│  (repetir até sim)   │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│   Tomar café         │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│  Abrir porta e sair  │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│  Deslocar ao trabalho│
└──────────┬───────────┘
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
  ESCREVA("Deslocar-se até o trabalho")
  ESCREVA("Chegar ao trabalho")
  ESCREVA("Passar o crachá na catraca")
FIM_ALGORITMO
```

---

## 2. 🔧 Troca de Pneu

> **Problema:** Descrever com segurança o processo de trocar um pneu furado na beira da estrada.

**Pontos de atenção:**
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
┌──────────────────────────┐
│  Buscar e posicionar     │
│        escada            │
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│  Remover lâmpada queimada │
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│  Verificar compatibilidade│◄──┐
│      da nova lâmpada     │   │
└──────────┬───────────────┘   │
           ↓                   │
┌──────────────────────────┐   │
│  Lâmpada ok? (repetir    │───┘
│  até compatível)         │
└──────────┬───────────────┘
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
  ESCREVA("Buscar a escada")
  ESCREVA("Posicionar a escada com segurança")
  ESCREVA("Subir / aproximar-se da lâmpada")
  ESCREVA("Girar a lâmpada no sentido anti-horário para remover")

  nova_lampada_ok <- FALSO

  ENQUANTO nova_lampada_ok = FALSO FAÇA
    ESCREVA("Verificar se a nova lâmpada é compatível")
    LEIA(nova_lampada_ok)
    ESCREVA("Buscar lâmpada com bocal e potência corretos")
  FIM_ENQUANTO

  ESCREVA("Instalar a nova lâmpada (sentido horário)")
  ESCREVA("Descer da escada")
  ESCREVA("Ligar o interruptor")
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
┌──────────────────────────┐
│   Recarregar o cartão    │
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│   Ir ao ponto de ônibus  │
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│  Aguardar ônibus correto │◄──┐
└──────────┬───────────────┘   │
           ↓                   │
┌──────────────────────────┐   │
│  É o ônibus correto?     │───┘
│  (repetir até sim)       │
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│  Aguardar parar + embarcar│
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│    Validar o cartão      │
└──────────┬───────────────┘
           ↓
┌──────────────────────────┐
│  Aguardar parada destino │◄──┐
└──────────┬───────────────┘   │
           ↓                   │
┌──────────────────────────┐   │
│  Chegou ao destino?      │───┘
│  (repetir até sim)       │
└──────────┬───────────────┘
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
  ESCREVA("Recarregar o cartão de transporte")
  ESCREVA("Deslocar-se até o ponto de ônibus")

  onibus_correto <- FALSO

  ENQUANTO onibus_correto = FALSO FAÇA
    LEIA(onibus_chegou, numero_onibus)
    ESCREVA("Aguardar próximo ônibus")
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
┌──────────────────────────┐
│  Verificar ingredientes  │◄──┐
└──────────┬───────────────┘   │
           ↓                   │
┌──────────────────────────┐   │
│  Todos disponíveis?      │───┘
│  (repetir até sim)       │
└──────────┬───────────────┘
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
┌──────────────────────────┐
│  Testar o palito         │◄──┐
└──────────┬───────────────┘   │
           ↓                   │
┌──────────────────────────┐   │
│  Palito sai limpo?       │───┘
│  (repetir até sim)       │
└──────────┬───────────────┘
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
    ESCREVA("Comprar ingredientes faltantes")
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
    ESCREVA("Assar por mais 10 minutos")
    tempo <- tempo + 10
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

**2. Repetição (estruturas de laço)**
Algumas etapas precisam ser feitas várias vezes até uma condição ser satisfeita. O palito no bolo só sai quando a massa estiver assada — não importa quantas tentativas.

**3. Validação antes de agir**
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
