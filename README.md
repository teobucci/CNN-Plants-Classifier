# Convolutional Neural Network: Plants Species Classification

This project was developed for the course of **Artificial Neural Networks and Deep Learning** for the MSc. in Mathematical Engineering at Politecnico di Milano, A.Y. 2022/2023.

## Description

```
.
├── README.md
├── misc
│   ├── accuracy_results.csv
│   ├── confusion.pdf
│   ├── ensemble_vgg16-resnet50.png
│   ├── single_augmentation.jpg
│   ├── supernet.pdf
│   └── ypred.npy
├── models
├── notebooks
│   ├── final_model.ipynb
│   ├── keras_tuner.ipynb
│   ├── metrics.ipynb
│   ├── supernet_choice.ipynb
│   └── supernet_histories
├── report
│   ├── bibliography.bib
│   ├── report.pdf
│   └── report.tex
├── requirements.txt
└── training_data_final
```

- [`final_model.ipynb`](notebooks/final_model.ipynb) is the main file that performs training and fine-tuning, and saves the models. Its decisions are partially based on the results from `supernet_choice.ipynb` and `keras_tuner.ipynb`. Finally, these models are evaluated in `metrics.ipynb`.
- [`keras_tuner.ipynb`](notebooks/keras_tuner.ipynb) provides the implementation of the Keras tuner code to tune the hyperparameters of the models.
- [`metrics.ipynb`](notebooks/metrics.ipynb) contains the code to evaluate the models and provide accuracies and F1-scores.
- [`supernet_choice.ipynb`](notebooks/supernet_choice.ipynb) performs a pilot run of transfer learning testing different pretrained models.
- [`accuracy_results.csv`](misc/accuracy_results.csv) contains a table of the accuracies of some of the models that we trained during the competition, it's included for the sake of completeness and as appendix in case the report explanations wouldn't be clear enough.

## Authors

- Paolo Botta ([@ploki99](https://github.com/ploki99))
- Teo Bucci ([@teobucci](https://github.com/teobucci))
- Silvia Caresana ([@silviacaresana](https://github.com/silviacaresana))

## Output

Check out the final [`report.pdf`](./report/report.pdf).

## License

[GNU GPLv3](https://choosealicense.com/licenses/gpl-3.0/)
