# Pràctica Kaggle APC UAB 2022-23
### Nom: Martí Rius Ollé 
### DATASET: Fetal Health Classification
### URL: https://www.kaggle.com/datasets/andrewmvd/fetal-health-classification?datasetId=916586&searchQuery=resampling)
## Resum
Aquest dataset classifica la salut fetal per prevenir la mortalitat infantil i materna.
## Context
La reducció de la mortalitat infantil es reflecteix en diversos dels Objectius de Desenvolupament Sostenible de les Nacions Unides i és un indicador clau del progrés humà.\
L'ONU preveu que l'any 2030, els països acabin amb les morts evitables de nounats i nens menors de 5 anys, i tots els països pretenen reduir la mortalitat dels menors de 5 anys com a mínim a 25 per cada 1.000 nascuts vius.

Paral·lelament a la noció de mortalitat infantil hi ha, per descomptat, la mortalitat materna, que suposa 295.000 morts durant i després de l'embaràs i el part (a partir del 2017). La gran majoria d'aquestes morts (94%) es van produir en entorns amb pocs recursos, i la majoria es podrien haver evitat.
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
Prenent l'atribut fetal_health com a objectiu volem avaluar la salut del fetus, permetent als professionals sanitaris prendre mesures per prevenir la mortalitat infantil i materna.
## Experiments
Durant aquesta pràctica hem realitzat diferents experiments.
### Preprocessat
No he hagut de tractar cap atribut com a tal; ja que no hi havia cap atribut null i tots eren float, però he aplicat un resampling; perquè l'atribut objectiu estava massa desproporcionat.\
També he fet un PCA.
### Model
| :-------------: |:-------------:| :-------------:| :-------------:|
| Model | Hiperparametres | Mètrica | Temps |
| -- | -- | -- | -- |
| Decision Tree |   -   | 94% | 0.0289s |
| Random Forest |   -   | 97% | 0.5944s |
| K-Nearest-Neighbor |   -   | 88% | 0.2045s |
| SVM | Kernel lineal | 84% | 7.4696s |
| SVM | Kernel rbf | 91% | 1.0173s |
| SVM | Kernel polinomial | 90% | 1971.87s |
## Conclusions
El model més eficaç que he aconseguit és el Random Forest amb un 97% d'acuracy. El segon amb més accuracy sense contar el decision tree òbviament seria el SVM amb el kernel rbf amb un 91%. Hi ha una diferència significativa.
## Idees per treballar en un futur
Es podria intentar trobar hyperparametres que milloressin l'acuracy dels models.
