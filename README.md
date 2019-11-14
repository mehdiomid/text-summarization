# Text Summarization
This is a project for text summarization by deep learning. The first project is to generate a summary from Amazon reviews.

Text summarization is a technique in natural language processing to generate a short, accurate, and fluent summary of a source document.

The Encoder-Decoder recurrent neural network architecture is currently recognized as a good technique for machine translation as well as text summarization. It is is being used when
there is a variable number of inputs, outputs or both inputs and outputs.

The decoder generates each word in the output sequence given two sources of information:

* Context Vector: The encoded representation of the source document provided by the encoder.

* Generated Sequence: The word or sequence of words already generated as a summary.

## Challenges:

* The development of separate encoder and decoder models combined into a pipeline would allow error to
 accumulate during the sequence generation process.

* The encoded input is used as context for generating each step in the output.
 Although this works, the fixed-length encoding of the input limits the length of output sequences.

* An extension of the Encoder-Decoder architecture is to provide a way to allow the decoder to learn where
 to pay attention to the encoded input when generating each step of the output sequence. This extension of the architecture is called attention.

## Word Embeddings:

Different types of encoders can be used, although more commonly bidirectional recurrent neural networks, such as LSTMs, are used. In cases where recurrent neural networks are used in the encoder, a word embedding is used to provide a distributed representation of words.