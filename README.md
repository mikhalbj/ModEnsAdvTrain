# Inclusion-Exclusion Enhanced Ensemble Adversarial Training

A project using Modified Ensemble Adversarial Training to defend against white and black box attacks. Group 6 Project for STOR 566.

Adversarial training is a state of the art technique used to enhance the robustness of deep learning models against testing-time attacks from perturbed images designed to fool them. Ensemble Adversarial Training, originally proposed by Tramer et al., creates adversarial images utilizing min max optimization over a probability simplex on multiple models simultaneously. Due to the transference property of adversarial images, this process tends to select images in the shared adversarial perturbation space of the models. This paper describes a novel application of Alternating Projected Gradient Descent Ascent method to find adversarial examples in the non-overlapping perturbation spaces of the various models. Our method yielded greater robustness against both white box and black box attacks, as well as non-perturbed images, than traditional adversarial training and Ensemble Adversarial Training.

<hr>

# Table of Contents
* [Team Members](#team-members)
* [Code Descriptions](#code-descriptions)

# <a name="team-members"></a>Team Members
* Henry Shugart <hshugart@email.unc.edu>
* Yeshavi Munagala <munagala@email.unc.edu>
* Mikhail Ben-Joseph <mikbenjo@live.unc.edu>
* Judy Chao <judychao@live.unc.edu>

# <a name="code-descriptions"></a>Code Descriptions

**APGDAImageCreation.ipynb**: Creates 50,000 adversarial images per model combination which are saved as a pkl file for easy access.

**BlackBox+WhiteBoxAttack**: Performs various forms of black and white box attack, including Fast Gradient Sign Method (FGSM) and Projected Gradient Descent (PGD). Plots comparative performance of models.

**EnsembleAdversarialTraining.ipynb**: Performs 256 epochs of traditional Ensemble Adversarial Training on VGG11. 

**ModifiedEAT.ipynb**: Performs 256 epochs of Ensemble Adversarial Training with the images derived from our modified APGDA approach. 

**TraditionalAT.ipnyb**: Performs 256 epochs of traditional Adversarial Training on pre-trained VGG11.
