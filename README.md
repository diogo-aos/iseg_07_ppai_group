# iseg_07_ppai_group

- Google Drive group folder
  - https://drive.google.com/drive/folders/1cD4X8e8InCirvHeAHGh65vIrEP9VvPPu
- clear notebook outputs
  - `jupyter nbconvert --ClearOutputPreprocessor.enabled=True --inplace xx.ipynb`

## Tasks
Exercise 1 -> Diogo
 1.a) Dados sintéticos
   1.a.i) Pipeline dados sintéticos [V]
   1.a.ii) Treinar modelos [V]
   1.a.ii) Gerar dados sintéticos para as 4 classes [V]
   1.a.iii) Avaliação dados sintéticos [V]
 1.b) Modelo
   1.b.i) Pipeline modelo - transfer learning - escolher modelo pretreinado [V]
   1.b.ii) Treinar em dados reais [V]
   1.b.iii) Treinar em dados sintéticos [V]
   1.b.iv) Treinar em dados reais + sintéticos [V]
   1.b.v) Compilar resultados [V]

Exercise 2
 2.a) Combinar tabelas [V]
 2.b) Dados anonamizados [V]
   2.b.i) Criar modelo de anonamização [V]
   2.b.ii) Transformar dados [V]
 2.c) Dados sintéticos [V]
   2.c.i) Pipeline para gerar dados com SDV, configurar constraints [V]
   2.c.ii) Gerar dados sintéticos [V]
 2.d) Modelo reais/sintéticos
   2.d.i) Pipeline modelo [V]
   2.d.ii) Treinar reais [V]
   2.d.iii) Treinar sintéticos (dependência 2.c) [V]
   2.d.iv) Compilar resultados reais (AUC ROC) [V]
   2.d.v) Compilar resultados sintéticos (AUC ROC) [V]
 2.e) Modelo anonamizados (dependência 2.b) [V]
   2.e.i) Pipeline modelo [V]
   2.e.ii) Treinar [V]
   2.e.iii) Compilar resultados (AUC ROC) [V]



## Tasks Exercise 1 - MRI Dementia
- data
  - https://www.kaggle.com/datasets/tourist55/alzheimers-dataset-4-class-of-images

![](ppai_group_01.jpeg)

## Tasks Exercise 2 - Credit Card Approval
- data:
  - https://www.kaggle.com/datasets/rikdifos/credit-card-approval-prediction

![](ppai_group_02.jpeg)


## Sources

- Exer 1
  - Transfer Learning
    - https://debuggercafe.com/brain-mri-classification-using-pytorch-efficientnetb0/
    - https://pytorch.org/vision/stable/models.html
    - https://pytorch.org/tutorials/beginner/transfer_learning_tutorial.html
  - Inception Score
    - https://github.com/sbarratt/inception-score-pytorch
    
- Exer 2
  - SDV custom constraits
    - https://sdv.dev/SDV/user_guides/single_table/custom_constraints.html