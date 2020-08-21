# transferLearning
<h3>Transfer Learning with PyTorch</h3>

The idea of Transfer Learning to utilize a neural network that has trained in other cases, then we make a little adjustment to our case. Transfer Learning also called the pre-trained model.

For example, we have trained a model to detect men's faces, now we just use that model to detect our new cases of girls' faces, right? In the machine, we have learned the line edges of their faces, then we just do a little adjustment to suit our cases.

**Step 1: Adaptation (Training Classifier)**
- Load a pretrained model
- freeze the feature extractor
- modify the classifier to our data, leave it unfreezed
- train only on the classifier

**Step 2: Fine-tuning**
- unfreeze some or all the layers
- retrain using a lower learning rate (let say, 10% of previous learning rate)
- repeat fine-tuning with lower learning rate if necessary

<br>

>*note: this project uses jcopdl*
