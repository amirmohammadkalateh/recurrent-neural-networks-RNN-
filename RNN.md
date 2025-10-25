# recurrent-neural-networks-RNN-
***

# Recurrent Neural Networks (RNNs) Architectures

Recurrent Neurons and Layers are fundamental components of **Recurrent Neural Networks (RNNs)**, which are specially designed to handle **sequential data** such as text, speech, or time series. The key feature of a recurrent layer is its ability to maintain an internal **memory** of previously processed inputs.

## The Core Concept: Recurrence and Memory 🧠

A recurrent neuron takes two inputs at any given time step ($t$):
1.  The **current input** ($X_t$).
2.  The **Hidden State** ($H_{t-1}$), which is the memory or summary of all inputs processed up until the previous time step.

* **Recurrent Layer:** It is essentially a **single layer** that is applied **repeatedly (recurrently)** across the time dimension of the input sequence.
* **Hidden State ($H_t$):** This is the "memory cell" that captures information from the past sequence and is passed forward to the next step.

## RNN Architecture Patterns (Illustrated) 🖼️

The image illustrates five common patterns used in RNN architectures, defined by the relationship between the number of **Inputs (Blue Blocks)** and **Outputs (Green Blocks)** over time.

| Pattern | Structure | Key Function | Conceptual Example |
| :--- | :--- | :--- | :--- |
| **1. One to One** | Single Input, Single Output. | Acts like a standard Feedforward Network (no sequence processing). | **Image Classification** (Input: 1 image, Output: 1 label). |
| **2. One to Many** | Single Input generates a sequence of Outputs. | The initial input is processed, and the subsequent outputs are generated based on the recurrent memory state. | **Image Captioning** (Input: 1 image, Output: A sequence of words/a sentence). |
| **3. Many to One** | A sequence of Inputs leads to a single Output. | The network processes the entire input sequence to arrive at a single summarizing result. | **Sentiment Analysis** (Input: A sequence of words/a sentence, Output: 1 label like "Positive" or "Negative"). |
| **4. Many to Many (Synchronous)** | Sequence of Inputs matches the Sequence of Outputs in length, with output generated at every step. | Used when an output is required for every corresponding input element. | **Sequence Tagging** (Input: Sentence, Output: A grammatical tag for every word). |
| **5. Many to Many (Asynchronous / Encoder-Decoder)** | Sequence of Inputs is processed entirely, and then a sequence of Outputs is generated. The input and output lengths may be different. | The first part (**Encoder**) compresses the input sequence into a **Context Vector**, and the second part (**Decoder**) generates the output sequence. | **Machine Translation** (Input: A sentence in Language A, Output: The translated sentence in Language B). |

***

As per your custom instructions, here are 10 sentences about the core topic (RNNs) to conclude:

Recurrent networks are specifically designed for sequential data processing. They utilize a hidden state to pass information from one time step to the next. This mechanism gives them a form of memory for past inputs. The hidden state is crucial for understanding context within a long sequence. Different sequence tasks require different input-output mapping patterns. These patterns dictate the overall architecture of the RNN model. The many-to-one architecture is perfect for sequence classification tasks. Conversely, the one-to-many model is used for generating new sequences. The encoder-decoder structure is the standard for complex sequence translation. All these structures leverage the core recurrent neuron to manage temporal dependencies.
