# HSI+CNN — Plant Disease Detection

CNN-based classification pipeline using HSI (Hyperspectral Imaging) preprocessing to detect plant leaf diseases, benchmarked across four public Kaggle datasets.

🔗 Notebook:https://www.kaggle.com/code/mokeshanandan/notebook85ae1b8f14
## Results

| Dataset | Source | Accuracy | F1-score |
|---|---|:---:|:---:|
| New Plant Diseases Dataset | vipoooool| 100% | 100% |
| PlantVillage Dataset |abdallahalidev	 | 100% | 100% |
| PlantDoc |nirmalsankalana | 91.22% | 89.92% |
| PlantVillage Dataset |emmarex/plantdisease	| 98.70% | 97.80% |

## Approach

- Backbone: <!-- TODO: your HSI preprocessing method + CNN architecture -->
- Data augmentation applied before training <!-- TODO: confirm/edit -->
- Evaluated on a held-out test split for each dataset, with accuracy/loss curves logged per run
- <!-- TODO: any dataset-specific notes, e.g. why PlantDoc scores lower -->

## Notes

- 
PlantVillage Dataset appears twice (rows 2 and 4), sourced from two different Kaggle uploads of the same underlying data, evaluated separately for consistency.


