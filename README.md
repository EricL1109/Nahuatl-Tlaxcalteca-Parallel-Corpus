# Spanish–Nahuatl_Tlaxcalteca Parallel Corpus

This repository presents a parallel corpus for Spanish–Nahuatl_Tlaxcalteca developed for research in Neural Machine Translation (NMT), Natural Language Processing (NLP), and low-resource language technologies.

## Parallel Database Generation

The Spanish–Tlaxcalan Nahuatl parallel database was specifically developed for machine translation and natural language processing tasks in a low-resource indigenous language. Due to the absence of structured digital resources for this regional Nahuatl variant, a complete process of data collection, digitization, cleaning, normalization, and linguistic alignment was designed.

The construction of the database involved multiple linguistic sources to ensure lexical diversity and dialectal representativeness. These sources include Spanish–Nahuatl bilingual dictionaries from the Tlaxcala region, educational materials, literary texts, everyday expressions provided by native speakers, and parallel resources such as the Axolotl corpus.

Printed documents were digitized using OCR tools such as Tesseract and EasyOCR. Subsequently, the texts underwent preprocessing stages including lexical cleaning, removal of special characters, sentence segmentation, and orthographic normalization according to the recommendations established by the Instituto Nacional de Lenguas Indígenas (INALI).

The alignment between Spanish and Tlaxcalan Nahuatl sentences was manually performed, prioritizing semantic equivalence and linguistic consistency. The final structure of the database was stored in JSON format using the fields `input_text` and `target_text`, allowing direct compatibility with Transformer-based architectures such as T5 and mT5.

The complete database contains 4,088 Spanish–Tlaxcalan Nahuatl bilingual pairs organized into thematic categories related to greetings, family, nature, education, traditions, and everyday expressions. For academic and research purposes, this GitHub repository provides a representative subset of 1,200 bilingual pairs from the complete corpus, enabling its use in machine translation, natural language processing, and digital preservation of low-resource indigenous languages.

## Experiment

The database was used to perform the fine-tuning process of the `t5-small-spanish-nahuatl` neural model based on the Transformer architecture. During training, different hyperparameter configurations were explored through grid search, evaluating combinations of epochs, learning rates, and batch sizes.

The experimental evaluation was conducted using BLEU, chrF, and TER metrics, which are widely used in neural machine translation. The best configuration achieved a BLEU score of 23.95 and a chrF score of 68.64, demonstrating that the proposed database significantly improves the performance of neural models applied to low-resource indigenous languages.

<img width="800" height="400" alt="results" src="https://github.com/user-attachments/assets/1924f5e8-617f-4079-9874-afa19bc02782" />


## Authors

* Nancy Galicia-Cocoletzi
* Eric Ramos-Aguilar
* Cecilia Reyes-Peña
* Ricardo Ramos-Aguilar

## Citation

Galicia Cocoletzi, N., Ramos Aguilar, E., & Reyes Peña, C. (2025). *Spanish–Tlaxcalan Nahuatl Parallel Corpus for Neural Machine Translation and Low-Resource Language Processing*. Zenodo. https://zenodo.org/records/19870065

## License

© 2025 Nancy Galicia Cocoletzi et al.

This dataset is licensed under the Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0) License.

You are free to:

* Share — copy and redistribute the material
* Adapt — remix, transform, and build upon the material

Under the following terms:

* Attribution — You must give appropriate credit to the original authors
* NonCommercial — You may not use the material for commercial purposes

This dataset is intended for research and educational use, particularly in the study of low-resource languages.

For more details: https://creativecommons.org/licenses/by-nc/4.0/

For commercial use or special permissions, please contact the authors:

* Nancy Galicia Cocoletzi ([nan.galicia03@gmail.com](mailto:nan.galicia03@gmail.com))
* Eric Ramos Aguilar ([eramosa@ipn.mx](mailto:eramosa@ipn.mx))
