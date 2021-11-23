# MINFO Speaker Identification
  
Based on a few hours of
data you can train ur model. The data we use is from Mini Librispeech + OpenRIR.

There are four files here:

* `train.py`: the main code file, outlines the entire training process.
* `train.yaml`: the hyperparameters file, sets all parameters of execution.
* `custom_model.py`: A file containing the definition of a PyTorch module.
* `mini_librispeech_prepare.py`: If necessary, downloads and prepares data manifests.

To train the speaker-id model, just execute the following on the command-line:

```bash
python train.py train.yaml
```

This will automatically download and prepare the data manifest for mini
librispeech, and then train a model with dynamically augmented samples.

[This project can be executed and tested here. You will get more details and explanation i provided](https://colab.research.google.com/drive/1TY_810bXDt1h7Iz7iXQ6xF5jZ1YJFFwL?usp=sharing)