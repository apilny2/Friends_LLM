# Friends Dialogue Language Model

This repository contains a PyTorch implementation of a simple language model trained on dialogues from the TV show "Friends." The model uses a Transformer-based architecture to predict the next character in a sequence, enabling the generation of new text based on the patterns learned from the input data.

## Features
- **Transformer Architecture**: Utilizes multiple layers of self-attention and feed-forward neural networks for sequence modeling.
- **Custom Data Loader**: Reads and processes a cleaned dialogue text file, encoding each character as an integer.
- **Training and Validation**: Splits the dataset into training and validation sets, with periodic evaluation of the model's performance.
- **Batch Processing**: Generates batches of data for efficient training using GPU acceleration if available.
- **Text Generation**: Generates new sequences of text based on a given context using the trained model.

## How to Use
1. **Upload the Dataset**: Ensure your cleaned dialogue file (`Friends.txt`) is available in the working directory.
2. **Run the Script**: Execute the provided Python script in a suitable environment (e.g., Google Colab) to train the model and generate text.
3. **Model Configuration**: Adjust hyperparameters such as `batch_size`, `block_size`, `learning_rate`, and model architecture parameters as needed.

## Example Output
The model generates new dialogue sequences in the style of "Friends" characters, capturing the show's conversational patterns.

```plaintext
Chandler:
Hey, how you doin'?

Joey:
I'm good! Just thinking about that new audition I have tomorrow.

Rachel:
Oh, Joey, you'll nail it, like you always do!
```
Feel free to experiment with the code and improve the model's performance or adapt it for other text-based datasets.

## Dependencies
- **PyTorch**
- **Pandas**

## Acknowledgements
Developed from Andrej Karpathy's work on character-level language models. All I did was use his code for the Shakespeare dataset. 

## Citation for data
```plaintext
Chen, S.Y., Hsu, C.C., Kuo, C.C. and Ku, L.W. EmotionLines: An Emotion Corpus of Multi-Party Conversations.
arXiv preprint arXiv:1802.08379 (2018).
```
