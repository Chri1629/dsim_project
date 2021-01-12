# Digital Signal & Image Management Project

Il progetto presente in questo repository si divide in tre sottoprogetti:

## Audio Classification

Questa sezione del progetto si occupa di identificare da una traccia audio di una persona, se quest'ultima stia effettivamente leggendo un testo oppure no, cercando di comprendere se il testo risulta quindi improvvisato oppure preparato in anticipo. In particolare sono state usate diverse tecniche:

- SVC: viene applicata una SVC sulle tracce audio. Le performance sono discrete ma migliorabili.
- MEL: si producono gli spettrogrammi di MEL e si sfruttano le CNN per fare classificazione immagini. In particolare si usano una rete pretrainata tagliata e a cui è stato aggiunto un classificatore logistico, una rete pretrainata a cui viene aggiunto un layer denso ed una rete CNN costruita da 0. Le performance migliori sono quelle ottenute dalla rete tagliata.

## Image Classification

La sezione di image Classification si occupa di riconoscere da un'immagine se essa rappresenta o meno un mezzo di emergenza (ambulanze, polizia, vigili del fuoco etc), distinguendo questi mezzi da quelli comuni. Sono state usate due reti per questo problema di classificazione. La prima rete è una CNN costruita da 0 mentre la seconda è una rete pretrainata sul task di imagenet. La rete che funziona meglio è la seconda.


## Image Retrieval 

In questa sezione vengono prese delle immagini di test prese da internet e si cercano all'interno del dataset utilizzato per la parte di classificazione immagini le immagini più simili a quelle di partenza. Le performance che si ottengono sono molto buone.
