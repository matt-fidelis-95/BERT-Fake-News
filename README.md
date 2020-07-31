# BERT-Fake-News
Neste trabalho é proposta uma abordagem para detectar notícias falsas utilizando o BERTimbau (BERT para português) com o treinamento em duas bases de dados fornecidas. Além disso são testadas outras duas abordagens envolvendo o Random Forests e o SVM.
Inicialmente foi feito um processo de limpeza manual das bases, após isso é feita uma tokenização, seguida da remoção de palavras de parada e, no caso do Random Forests e do SVM, uma conversão das palavras para vetores usando a parametrização TF-IDF.
A divisão entre os dados de teste e treinamento se fez através de holdout, com 70% do conjunto pertencendo ao treinamento e 30% ao teste.
O ajuste fino do BERT foi feito utilizando 5 épocas de treinamento, um learning rate de 3e-5 e um batch size de tamanho 4.
Para o caso do SVM foi utilizado um kernel linear e um parâmetro de regularização de 1.0.
Para o caso do Random Forests foram utilizadas 100 árvores de treinamento.
