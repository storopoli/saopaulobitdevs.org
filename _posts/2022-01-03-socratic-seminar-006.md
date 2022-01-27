---
layout: post
type: socratic
title: "Seminário Socrático 006"
meetup: https://www.meetup.com/pt-BR/bitdevsemportugues/
---

Detalhes sobre o local do evento aqui: [https://www.meetup.com/pt-BR/bitdevsemportugues/events/283448461/](https://www.meetup.com/pt-BR/bitdevsemportugues/events/283448461/)

## Anúncios

- Entrem no grupo do Telegram "[Bitdevs em Português](https://t.me/joinchat/lHusQ1bV9fUyNDY5)" para ajudar na curadoria dos encontros!
- Nessa edição, a discussão será inteiramente dedicada a um aprofundamento no tema "Covenants", por isso não teremos updates relacionados a Pull requests, e-mails da mailing list, etc.

## Covenants

- [Definição do termo Covenants](https://www.investopedia.com/terms/c/covenant.asp)
- [Covenants no contexto do Bitcoin](https://bitcoinops.org/en/topics/covenants/)

### História

- [Origem do termo - Primeira menção por Greg Max](https://bitcointalk.org/index.php?topic=278122.0)
- [Discussões iniciais sobre Covenants](https://download.wpsoftware.net/bitcoin/wizards/2014/01/14-01-15.log)
- [Primeira formalização e a ideia de "Vaults" por Moser-Eyal-Sirer](https://maltemoeser.de/paper/covenants.pdf)

### Introdução

- [Algumas revisões conceituais - Recursive vs non-recursive / Fully enumerated vs Open ended / Client vs Consensus validation](https://rubin.io/bitcoin/2021/12/04/advent-7/)
- [As diferentes propostas de Covenants](https://rubin.io/blog/2021/07/02/covenants/)

### OP_CSFS e OP_CAT

- [Melhorando transações de Bitcoin com Covenants - RO'Conner&Piekarska](https://fc17.ifca.ai/bitcoin/papers/bitcoin17-final28.pdf)
- [Covenants na Elements (Liquid)](https://blog.blockstream.com/en-covenants-in-elements-alpha/)
- [Sugestão para BIP - Seguir thread com resposta do O'Conner](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2021-July/019192.html)
- [OP_CAT e truques com Schnorr](https://medium.com/blockstream/cat-and-schnorr-tricks-i-faf1b59bd298) / [Parte 2](https://medium.com/blockstream/cat-and-schnorr-tricks-ii-2f6ede3d7bb5)

### Anyprevout 

- [BIP 118](https://github.com/bitcoin/bips/blob/master/bip-0118.mediawiki)
- [Eltoo](https://blockstream.com/eltoo.pdf)
- [Vaults com Anyprevout?](http://yakshaver.org/2021/11/18/covenants.html)
- [Status Eltoo/Tasks](https://yakshaver.org/bitcoin/#eltoo)
- [Branch AJ Towns - Anyprevout](https://github.com/ajtowns/bitcoin/commits/202101-anyprevout)
- [Esboço Eltoo AJ](https://lists.linuxfoundation.org/pipermail/lightning-dev/2019-May/001996.html)
- [Implementação experimental do Eltoo por R. Meyers](https://lists.linuxfoundation.org/pipermail/lightning-dev/2019-September/002131.html)
- [Alguns dos benefícios do Eltoo (não necessidade de armazenar estados antigos) com PTLC](https://lists.linuxfoundation.org/pipermail/lightning-dev/2021-October/003278.html)

### OP_CTV

- [BIP 119](https://github.com/bitcoin/bips/blob/master/bip-0119.mediawiki)
- [PR implementação OP_CTV Bitcoin Core](https://github.com/bitcoin/bitcoin/pull/21702)
- [Use cases e Sapio no Advent Calendar](https://rubin.io/advent21/) + [Use cases no utxos.org](https://utxos.org/uses/)
- [Reunião #01 - BIP 119](https://gnusha.org/ctv-bip-review/2022-01-11.log) - [Resumo](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2022-January/019744.html)
- [Resumo OP_CTV por Namcios na Bitcoin Magazine](https://bitcoinmagazine.com/technical/what-is-bitcoin-checktemplateverify)
- [OP_CTV e DLCs](https://mailmanlists.org/pipermail/dlc-dev/2022-January/000102.html)
- [Eltoo possível com OP_CTV + OP_CSFS?](https://github.com/bitcoin/bips/blob/master/bip-0119.mediawiki#Eltoo_with_OP_CHECKSIGFROMSTACKVERIFY) + [Comparação com a construção por Anyprevout](https://bitcoin.stackexchange.com/questions/111497/how-do-eltoo-channel-constructions-using-anyprevout-compare-to-those-using-ctv-a)
- [Aprenda Sapio](https://learn.sapio-lang.org/)

### Debate
- [Debate do J. Rubin com A. Poelstra na Tabconf - Recursive vs non-recursive - OP_CTV limitado?](https://gist.github.com/JeremyRubin/2d69841755cf048f0c45bef8edf63b4c)
- [Preocupações do Michael Folkson + Peter Todd](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2022-January/019738.html) / [Resposta do J. Rubin](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2022-January/019739.html)
- [Poinsot a favor do status quo e priorização do Anyprevout](https://twitter.com/darosior/status/1474375244991369218)
- [Timing Eltoo?](https://twitter.com/RyanTheGentry/status/1476326244555771904)
- [Opcodes para Vaults é uma área nascente de pesquisa...](https://twitter.com/michaelfolkson/status/1474763710300368897)
- [Review do Luke](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2022-January/019776.html) / [Resposta do J. Rubin](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2022-January/019781.html)

### OP_TLUV

- [Proposta do AJ na mailing list](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2021-September/019419.html)
- [Análise de J. Rubin](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2021-September/019424.html)

## TXHASH + CHECKSIGFROMSTACKVERIFY no lugar de CTV e ANYPREVOUT

- [Nova proposta do O'Connor](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2022-January/019813.html)
- [Resposta J. Rubin](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2022-January/019814.html)

### As diferentes alternativas - Trade offs

- [Três formas de controlar o futuro](https://arxiv.org/pdf/2006.16714.pdf)
- [Alternativas de design](https://utxos.org/alternatives/)
- ["Roadmap" - Por que não TLUV ou Anyprevout?](https://rubin.io/bitcoin/2021/12/24/advent-27/)
- [Protocolos de custódia usando Vaults](https://arxiv.org/pdf/2005.11776.pdf)
