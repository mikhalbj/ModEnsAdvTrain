# ModEnsAdvTrain
A project using Modified Ensemble Adversarial Training to defend against white and black box attacks. Group 6 Project for STOR 566.


**APGDAImageCreation.ipynb**: Creates 50,000 adversarial images per model combination which are saved as a pkl file for easy access.

**BlackBox+WhiteBoxAttack**: Performs various forms of black and white box attack, including Fast Gradient Sign Method (FGSM) and Projected Gradient Descent (PGD). Plots comparative performance of models.

**EnsembleAdversarialTraining.ipynb**: Performs 256 epochs of traditional Ensemble Adversarial Training on VGG11. 

**ModifiedEAT.ipynb**: Performs 256 epochs of Ensemble Adversarial Training with the images derived from our modified APGDA approach. 

**TraditionalAT.ipnyb**: Performs 256 epochs of traditional Adversarial Training on pre-trained VGG11.
