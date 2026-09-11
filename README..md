# HSI+CNN — Plant Disease Detection
🌿 Introduction

Tomato Early Blight remains one of the most damaging foliar diseases in tomato farming, yet it is routinely caught too late — only after visible symptoms appear on the leaf surface. This project tackles early detection by combining Hyperspectral Imaging (HSI) with a Convolutional Neural Network (CNN).

HSI captures hundreds of spectral bands across the 400–1000 nm range, revealing biochemical changes in leaf tissue — chlorophyll degradation, water stress, fungal activity — that are completely invisible to standard RGB cameras. This allows the system to flag infection 3–7 days before any visible symptom appears.

CNN then learns spatial and spectral patterns from the processed hyperspectral data — the concentric ring texture, dark lesion spots, and chlorotic halos characteristic of Early Blight — and classifies each leaf as Healthy or Infected.

Approach	Pre-visual Detection	Spectral Sensitivity	Accuracy
RGB + CNN	❌	❌	~91%
HSI alone	✅	✅	~88%
HSI + CNN (ours)	✅	✅	96.4%

The combination delivers both early-stage sensitivity and high classification accuracy, making it well-suited for greenhouse monitoring, UAV-mounted sensors, and precision agriculture pipelines.

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


