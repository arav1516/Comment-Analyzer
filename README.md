# Comment-Analyzer
The model weights are present in the model.weights.h5 file in the drive.
Till now this is what the project is able to do
1] Given the video id for a particular video the code first collects the 100 recent most comments on that video.
2] Processes the comments into plain text so that they can be fed into the bert preprocessing model.
3] Since I am using BERT model to vectorize my input text therefore the text is then fed into the BERT preprocessor which then feeds the preprocessed text into the BERT model.
4] After getting the output vector from the BERT model the output is fed into the neural network which is already trained. (The loss function used in training is BinaryCrossEntropy).
5] The model gives an output which then has to converted to a value between 0 and 1 using sigmoid.
6] If the value is closer to 0 it should be a negative comment and if the value is closer to 1 it should be a positive comment.
