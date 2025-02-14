# Deep RNN for music generating

This project is based on Deep Improvisation project: https://github.com/tatsuyah/deep-improvisation
Easy-to-use Deep LSTM Neural Network to generate song like containing improvisation.

[Sample sound tracks (SoundCloud)](https://soundcloud.com/user-259574192/generated-song2)


## Packages needed

 - Keras
 - TensorFlow
 - Python MIDI (To install MIDI for python3, run: pip install git+https://github.com/vishnubob/python-midi@feature/python3)

## Usage:

  #### 1. Convert MIDI file to text

  ```
  python ./src/parse_midi_to_text.py
  ```

  #### 2. Train the model (Tensorflow backend is used by default, and it uses GPU)

  ```
  python ./src/training.py
  ```

  #### 3. Generate music

  ```
  python ./src/generate_music.py
  ```

## Note

   You can use any music midi file to train an RNN model, however, you should use pure music without lyrics or singer, for example, I used piano plays as training data.

## License

MIT © [Tatsuya Hatanaka](https://github.com/tatsuyah)