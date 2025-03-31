
2025-02-04 14:53

Status:

Tags: [[blockchain]] [[incomplet - incomplete]]


# Asynchronous Byzantine Fault Tolerence

Dans un aBFT, le réseau autorise certains messages d'être perdus à jamais, ou retardé à jamais.
Il ne pose aucune hypothèse sur le temps à partir du quel un accord est conclu.
#lacune-gap

L'avantage majeure réside dans le fait que le réseau est plus résistant en cas de ralentissement ou interruption du réseau.

### Charactéristiques d'un réseau aBFT:
- Asynchronisme : Aucune hypothèse sur la synchronisation des messages ou les retards du réseau.
- Tolérance aux pannes byzantines : Capacité à résister à des défaillances arbitraires (byzantines), y compris à des comportements malveillants.
- Consensus éventuel : Garantie que tous les nœuds honnêtes finiront par se mettre d'accord sur l'ordre des transactions.
- Évolutivité : Souvent plus évolutive que les systèmes BFT synchrones.

### Fonctionnement:
- Propagation des messages : Les nœuds diffusent des messages (transactions ou blocs) dans le réseau.
- Vote à plusieurs tours : Les nœuds participent à plusieurs tours de vote sur l'ordre et la validité des messages.
- Formation du quorum : Un nombre suffisant de nœuds doit se mettre d'accord pour parvenir à un consensus.
- Finalité : Une fois le consensus atteint, la décision est considérée comme définitive et irréversible.
- Fonctionnement continu : Le processus se répète pour chaque nouvelle série de messages ou de blocs.

Résilience : Fonctionnement continu même avec un certain pourcentage de nœuds défectueux ou malveillants.

Traduit avec DeepL.com (version gratuite)

cf: What is Hedera Hashgraph

## Références:

[[Byzantine Fault Tolerance]]