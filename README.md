# U.S. English Kaldi Profile

A [Rhasspy](https://github.com/rhasspy/rhasspy) profile for U.S. English (`en`).

Includes:

* A [Kaldi nnet3](https://kaldi-asr.org/doc/dnn3.html) speech to text model
    * See files in `acoustic_model/`
    * Recipe created with [ipa2kaldi](https://github.com/rhasspy/ipa2kaldi)
    * Word error rate: 5.90%
    * Trained on:
        * [Common Voice](https://commonvoice.mozilla.org) (1,449 hours)
        * [LibriSpeech](http://www.openslr.org/12/) (363 hours)
        * [M-AILabs](https://www.caito.de/2019/01/the-m-ailabs-speech-dataset/) (98 hours)
        * [Tatoeba](https://tatoeba.org) (185 hours)
        * [VCTK](https://datashare.ed.ac.uk/handle/10283/3443) (41 hours)
        * [Voxforge](http://voxforge.org/en) (124 hours)
* An [IPA](https://en.wikipedia.org/wiki/International_Phonetic_Alphabet) pronunciation lexicon based on [Reece Dunn's](http://www.reecedunn.co.uk/) U.S. English lexicon
    * See `base_dictionary.txt.gz`
* A [phonetisaurus](https://github.com/AdolfVonKleist/Phonetisaurus) grapheme to phoneme model for predicting word pronunciations
    * See `g2p.fst.gz`
    * Trained on `base_dictionary.txt.gz`
* A tri-gram [ARPA language model](https://cmusphinx.github.io/wiki/arpaformat/)
    * See `base_language_model.txt.gz`
    * Text from audio transcriptions, [Common Voice](https://github.com/mozilla/common-voice/tree/master/server/data/en), and [Universal Dependencies](https://universaldependencies.org/)
