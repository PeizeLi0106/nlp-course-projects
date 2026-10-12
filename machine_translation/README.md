# Neural Machine Translation

A two-person NLP course project exploring recurrent
encoder–decoder models and pretrained translation models.

## Dataset

The notebooks use Europarl v7 English–Dutch and English–Swedish
parallel corpora. Dataset files are not included in this repository.

Expected local structure:

data/
├── europarl-v7.nl-en.en
├── europarl-v7.nl-en.nl
└── sv-en/
    ├── europarl-v7.sv-en.en
    └── europarl-v7.sv-en.sv

## Notebooks

1. task1_dataExploration.ipynb — corpus exploration and sampling.
2. task2_preprocessing.ipynb — preprocessing and aligned sampling.
3. task3_translation.ipynb — GRU translation models and embedding experiments.
4. task4_attention.ipynb — translation with additive attention.
5. task5_pivotTranslation.ipynb — Dutch–English–Swedish MarianMT translation.

Run task2 before task3 and task4. It generates:
- data/preprocessed_10_percent.en
- data/preprocessed_10_percent.nl

Task5 reads the original Dutch–English and Swedish–English files.

## Running the Notebooks

Dependencies are listed in requirements.txt. Package-version
compatibility has not yet been verified in a fresh environment.

Open the notebooks in Jupyter with the working directory set to
machine_translation/notebooks, so the relative data paths resolve.

Run cells from top to bottom within each notebook.
MarianMT requires internet access to download pretrained models.
Training benefits from a GPU and may take substantially longer
on a CPU.

## Results

- Adding attention to the English–Dutch GRU model improved
  test BLEU from 5.78 to 11.59.
- Fine-tuning the MarianMT pivot pipeline improved
  Dutch–Swedish BLEU from 17.62 to 25.65 on 2,000 held-out examples.

These are separate experiments with different evaluation sets
and should not be compared directly.

See the [project report](reports/machine_translation_report.pdf)
for the recurrent-model experiments. The pivot-translation
experiment and its results are documented in task5.

## Limitations

These are coursework experiments rather than production systems.
Training outputs and model checkpoints are excluded from Git.