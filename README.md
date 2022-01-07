# -Cryptocurrency_Price_Prediction

Le but de ce projet est d'apprendre et de monter en compétence en machine learning/ deep learning afin accomplir les missions suivantes.
-Etudier la possibilité de prédiction d'une cryptomonnaie ou d'un panier de crypto
-Trouver des variables externes pour ajouter du signal,
-Backtester votre stratégie sur une cryptomonnaie avec votre modèle.

C'est intéressant de faire "peser" sur notre modèle un signal qui témoignerait d'un engouement ponctuel, ce qui améliorerait notre modèle contre la grande imprévisibilité/volatilité des cryptomonnaies.

J'ai rapidement regardé des codes de prédictions de cryptomonnaie que je ne comprenais pas. J'ai alors commencé à regarder certaines ressources pour comprendre chaque étape des modèles de prédiction. Je me suis ensuite initié à tensorflow avec le youtuber Thibaul Neveu ainsi qu'en effectuant le tutoriel de TensorFlow calssification d'images pour savoir comment coder les notions que j'ai apprises.

Nous avons choisis de prédire le cours d'Ethereum avec le modèle LSTM qui fait partis des réseaux récurrents qui peuvent modéliser des séries temporelles. Ainsi notre modèle pour prédire le prix de l'Ethereum ce jours ci va se employer sur le prix de l'ETH des cinq derniers jours.

Nous avons décidé de prendre le prix du BITCOIN comme signal externe en mettant son cours en entrée dans notre modèle LSTM. Nous avons choisi cet indicateur car le cours du BTC est souvent à l'initiative de mouvements de marché.

Nous avons fais varier les hyper paramètres pour avoir une erreur minimale. Nous avons augmenté les trainings à 400 et les neuronnes, les prédictions étaient moins précises et prenaient du temps, ce qui veut dire que nous étions tombés dans le surentrainement. C'est à ce moment où nous avons reperé l'overfitting que nous devons ajuster l'hyperparamètre dropout.

Nous avons essayé le modèle GRU qui fait aussi partis des réseaux récurrents. Ce dernier modèle nous a permis de réduire par deux l'erreur absolue de nos prédictions lorsque nous avions pas ajusté l'overfitting.



Ressources: https://www.tensorflow.org/tutorials/keras/classification chaines youtube Thibault Neveu, Neuraline ,
            livre intelligence artificielle vulgarisée - Le Machine Learning et le Deep Learning par la pratique de Aurélien VANNIEUWENHUYZE
            
            
