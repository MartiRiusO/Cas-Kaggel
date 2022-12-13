# Pràctica Kaggle APC UAB 2022-23
### Nom: Martí Rius Ollé ### DATASET: Fetal Health Classification
### URL: https://www.kaggle.com/datasets/andrewmvd/fetal-health-classification?datasetId=916586&searchQuery=resampling)
## Resum
Aquest dataset classifica la salut fetal per prevenir la mortalitat infantil i materna.
## Atributs
El datasset conté 22 atributs dels quals 21 són numèrics i 1 és categòric (fetal_health; el target).\
Els atributs són els següents:

- baseline value: Freqüència cardíaca fetal de referència (FHR) (batecs per minut)\
- accelerations: Nombre d'acceleracions per segon\
- fetal_movement: Nombre de moviments fetals per segon\
- uterine_contractions: Nombre de contraccions uterines per segon\
- light_decelerations: Nombre de LDs per segon (lleugeres desacceleracions)\
- severe_decelerations: Nombre de SDs per segon (desacceleracions severes)\
- prolongued_decelerations: Nombre de PDs per segon (desacceleracions prolongades)\
- abnormal_short_term_variability: Percentatge de temps amb variabilitat anormal a curt termini\
- mean_value_of_short_term_variability: Valor mitjà de la variabilitat a curt termini\
- percentage_of_time_with_abnormal_long_term_variability: Percentatge de temps amb variabilitat anormal a llarg termini\
- mean_value_of_long_term_variability: Valor mitjà de la variabilitat a llarg termini\
- histogram_width: Amplada de l'histograma fet utilitzant tots els valors d'un registre\
- histogram_min: Valor mínim de l'histograma\
- histogram_max: Valor màxim de l'histograma\
- histogram_number_of_peaks: Nombre de pics a l'histograma\
- histogram_number_of_zeroes: Nombre de zeros a l'histograma\
- histogram_mode: Mode de l'histograma\
- histogram_mean: Mitjana de l'histograma\
- histogram_median: Mediana de l'histograma\
- histogram_variance: Variància de l'histograma\
- histogram_tendency: Tendència de l'histograma\
- fetal_health: Normal=1 - Suspect=2 - Pathological=3 (Atribut objectiu)
### Objectius del dataset
Volem aprender quina és la ...
## Experiments
Durant aquesta pràctica hem realitzat diferents experiments.
### Preprocessat
Quines proves hem realitzat que tinguin a veure amb el pre-processat? com han afectat als resultats?
### Model
| Model | Hiperparametres | Mètrica | Temps |
| -- | -- | -- | -- |
| [Random Forest](link) | 100 Trees, XX | 57% | 100ms |
| Random Forest | 1000 Trees, XX | 58% | 1000ms |
| SVM | kernel: lineal C:10 | 58% | 200ms |
| -- | -- | -- | -- |
| [model de XXX](link al kaggle) | XXX | 58% | ?ms |
| [model de XXX](link al kaggle) | XXX | 62% | ?ms |
## Demo
Per tal de fer una prova, es pot fer servir amb la següent comanda
``` python3 demo/demo.py --input here ```
## Conclusions
El millor model que s'ha aconseguit ha estat...
En comparació amb l'estat de l'art i els altres treballs que hem analitzat....
## Idees per treballar en un futur
Crec que seria interesant indagar més en...
## Llicencia
El projecte s’ha desenvolupat sota llicència ZZZz.
