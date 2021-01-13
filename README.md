# Digital Signal & Image Management Project

Il progetto presente in questo repository si divide in tre sottoprogetti:

## Audio Classification

Questa sezione del progetto si occupa di identificare da una traccia audio di una persona se quest'ultima stia effettivamente leggendo un testo oppure no, cercando di comprendere tonalità improvvisate rispetto a quelle di una lettura. In particolare sono state utilizzare due tecniche:

- **SVM**: Sulle tracce audio viene applicata una Support Vector Machine e successivamente vengono analizzati i risultati in un classification report e una matrice di confusione.

- **Spettrogrammi di MEL**: dalle tracce audio vengono generati gli spettrogrammi di MEL, immagini che vengono utilizzate per addestrare delle reti neurali. In particolare si usano una rete pretrainata tagliata e a cui è stato aggiunto un classificatore logistico, una rete pretrainata a cui viene aggiunto un layer denso e una rete CNN costruita da 0.

## Image Classification

La sezione di Image Classification si occupa di riconoscere da un'immagine se essa rappresenta o meno un mezzo di emergenza (ambulanze, polizia, vigili del fuoco etc), distinguendo questi mezzi da quelli comuni. Sono state utilizzate due reti per questo problema di classificazione. La prima rete è una **CNN definita da noi** mentre la seconda è una rete **pretrainata** sul task di imagenet.


## Image Retrieval 

Nella seguente sezione vengono utilizzate delle immagini di test prese da internet e si cercano all'interno del dataset in possesso usato per la parte di classificazione immagini quelle più simili.
