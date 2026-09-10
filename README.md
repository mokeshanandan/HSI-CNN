# HSI+CNN — Plant Disease Detection

Deep learning model for plant disease classification using an HSI (Hyperspectral Imaging) preprocessing pipeline combined with a CNN classifier. Trained and evaluated across multiple public plant disease datasets.

## Model

- **Architecture:** HSI + CNN <!-- TODO: add specific backbone/layers, input size, params -->
- **Framework:** <!-- TODO: TensorFlow / PyTorch -->
- **Task:** Multi-class plant leaf disease classification

## Datasets & Results

Evaluated on 4 public datasets, benchmarked against a YOLOv8+CNN model (see [companion repo](#) <!-- TODO: link your YOLOv8+CNN repo here -->):

| # | Dataset | HSI+CNN Accuracy | HSI+CNN F1 | YOLOv8+CNN Accuracy | YOLOv8+CNN F1 |
|---|---------|:---:|:---:|:---:|:---:|
| 1 | [New Plant Diseases Dataset](#) <!-- TODO: Kaggle link --> | 100% | 100% | 49.50% | 100% |
| 2 | [PlantVillage Dataset](#) <!-- TODO: Kaggle link --> | 100% | 100% | 99.36% | 62.13% |
| 3 | [PlantDoc](#) <!-- TODO: Kaggle link --> | 91.22% | 89.92% | 100% | 100% |
| 4 | [PlantVillage Dataset](#) <!-- TODO: Kaggle link (specify variant if different from #2) --> | 98.70% | 97.80% | 99.10% | 96.80% |

![Confusion Matrix](results/confusion_matrix.png)
![Accuracy / Loss Curve](results/accuracy_loss_curve.png)
![Sample Predictions](results/sample_predictions.png)

## Prototype

An interactive HTML prototype is included in [`prototype/`](prototype/), showing live training curves and prediction demos for the model.

- `prototype/hsi_cnn_plantvillage.html` — PlantVillage dataset demo
- `prototype/hsi_cnn_ip102.html` — IP102 dataset demo <!-- TODO: confirm this dataset name/purpose -->

Open either file directly in a browser to view the interactive demo, or enable **GitHub Pages** on this repo to host it as a live link.

## Repository Structure

```
HSI-CNN/
├── README.md
├── notebooks/
│   └── training_notebook.ipynb
├── results/
│   ├── confusion_matrix.png
│   ├── accuracy_loss_curve.png
│   └── sample_predictions.png
├── prototype/
│   ├── hsi_cnn_plantvillage.html
│   └── hsi_cnn_ip102.html
├── requirements.txt
└── LICENSE
```

## How to Run

```bash
pip install -r requirements.txt
python train.py
```

<!-- TODO: adjust to your actual entry-point script/notebook name -->

## Files

| File | Description |
|------|-------------|
| `notebooks/training_notebook.ipynb` | Model training and evaluation |
| `results/` | Confusion matrix, training curves, sample predictions |
| `prototype/` | Interactive HTML demo prototype |
| `requirements.txt` | Python dependencies |

## Citation

If you use this work, please cite:

> <!-- TODO: your paper citation once published/preprinted -->

Datasets used:
> <!-- TODO: add Kaggle dataset citations, e.g.:
> Bhattarai, S. (2018). New Plant Diseases Dataset (Augmented). Kaggle. -->

## License

MIT — see [LICENSE](LICENSE).
