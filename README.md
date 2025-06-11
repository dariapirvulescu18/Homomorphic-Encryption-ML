# Criptarea homomrfică în învățarea automată

Repoul conține codul integral al lucrării de licență _Uilizarea Criptositemelor Homomorfice pentru Securizarea datelor folosite în Învățarea Automată_ din cadrul Facultății de Matematică și Informatică, specializare Informatică, Coordonator științific: Conf.dr. Ruxandra Olimid.


## Structura
Se explorează doua biblioteci criptografice [OpenFHE](https://github.com/openfheorg/openfhe-python) și [ConcreteML](https://github.com/zama-ai/concrete-ml) (dezvoltat de Zama). Codul este scris în Python. Setul de date este luat de pe platforma [Kaggle](https://www.kaggle.com/dsv/10892812) și prelucrat în [notebook-ul](https://github.com/dariapirvulescu18/Homomorphic-Encryption-ML/blob/master/OpenFHE/data/process_data.ipynb). 

### OpenFHE
- Folderul [code](https://github.com/dariapirvulescu18/Homomorphic-Encryption-ML/tree/master/OpenFHE/code) conține implementarea unei regresii liniare si a unei regresie logistice; implementarea pe date clare și pe date criptate se afla în notebook-uri separte în folderele aferente; in cadrul regresiei liniare se află și implementarea folosind [bootstraping](https://github.com/dariapirvulescu18/Homomorphic-Encryption-ML/blob/master/OpenFHE/code/liniar_regression/liniar_regression_bootstraping.ipynb), dar și experimentul pentru [verificarea stabilității CKKS-ului](https://github.com/dariapirvulescu18/Homomorphic-Encryption-ML/blob/master/OpenFHE/code/liniar_regression/li_r_trained_on_clear_data_pred_on_encrypted_data_5round_compare.ipynb).

- Folderul [data](https://github.com/dariapirvulescu18/Homomorphic-Encryption-ML/tree/master/OpenFHE/data) conține prelucrarea datelor.

- Folderul [plots](https://github.com/dariapirvulescu18/Homomorphic-Encryption-ML/tree/master/OpenFHE/plots) conține rezultatele în format .png pentru o mai bună vizualizare.

### Zama-ConcreteML
- Folderul [code](https://github.com/dariapirvulescu18/Homomorphic-Encryption-ML/tree/master/Zama-ConcreteML/code) conține implementarea unei regresii liniare și a unei regresie logistice; implementarea pe date clare si pe date criptate se afla în aceleași notebook-uri în folderele aferente; pentru regresia liniara este prezentată doar inferența pe date criptate, din cauza limitărilor impuse de bibliotecă; se gasește și implementarea din scikit-learn.

- Folderul [data](https://github.com/dariapirvulescu18/Homomorphic-Encryption-ML/tree/master/OpenFHE/data) conține prelucrarea datelor.

- Folderul [plots](https://github.com/dariapirvulescu18/Homomorphic-Encryption-ML/tree/master/OpenFHE/plots) conține rezultatele în format .png pentru o mai bună vizualizare.


## Surse de inspirație

- https://docs.pytorch.org/docs/stable/generated/torch.optim.SGD.html

- https://docs.zama.ai/concrete-ml

- https://github.com/zama-ai/concrete-ml/tree/main/docs/advanced_examples

- https://github.com/openfheorg/openfhe-python

- https://github.com/openfheorg/python-svm-examples

- https://github.com/openfheorg/python-log-reg-examples

- https://github.com/OpenMined/TenSEAL/blob/main/tutorials/Tutorial%201%20-%20Training%20and%20Evaluation%20of%20Logistic%20Regression%20on%20Encrypted%20Data.ipynb




