# Bidrectional LSTM RNN

RNN based on orignal machine learning project by Tyler Doll, Izaak Sulka, and Jeff Greene found here https://github.com/tylerdoll/music-generator

Training:
Call `python3 train.py --name <name of model to train> --songs_dir <directory containing midis>`
Optional params include:
    `--checkpoint <hdf5 file>` to resume training from a previous checkpoint.
    `--notes <pickled notes file>` to use pre-parsed notes.
    `--epochs <int>` to set the number of epochs to train for, defaults to 10

Predicting/Generating:
Call `python3 predict.py <name of model>` where model name is:
    - ragtime
    - rap
    - christmas
Or a custom trained model.

Note that a hdf5 and notes file must exist in their respective places with the same name to
generate a song.
