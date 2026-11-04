---
module: A01
tags: [ai, notebook]
---

# A01 · AI General Knowledge

> Know what you're talking about, and talk about it accurately.

[[00 Home|← Back to home]] · [[Glossary]] · [[Resources]]

## A01.01 · Tell apart AI, machine learning, deep learning and generative AI

- [x] A01.01 Tell apart AI, machine learning, deep learning and generative AI

> [!tip] Hint
> Four nested circles. Draw the diagram in your notebook.

**My notes:**
![[Pasted image 20261102024504.png]]

**Artificial intelligence:** Artificial intelligence (AI) is the capability of computational systems to perform tasks typically associated with human intelligence, such as learning, reasoning, problem-solving, perception, and decision-making. It is also a field of research spanning computer science, engineering, and mathematics that develops and studies methods and software enabling machines to perceive their environment and use learning and intelligence to take actions that maximise their chances of achieving defined goals.

**Machine learning:** Machine learning (ML) is a field of study in artificial intelligence concerned with the development and study of statistical algorithms that can learn from data and generalize to unseen data, and thus perform tasks without being explicitly programmed.

**Neural networks:** A neural network consists of connected units or nodes called artificial neurons, which loosely model the neurons in the brain. These are connected by edges, which model the synapses in the brain. Each artificial neuron receives signals from connected neurons, then processes them and sends a signal to other connected neurons. The "signal" is a real number, and the output of each neuron is computed by some non-linear function of the totality of its inputs, called the activation function. The strength of the signal at each connection is determined by a weight, which adjusts as part of the training process.

**Deep learning:** In machine learning, deep learning (DL) focuses on utilizing multilayered neural networks to perform tasks such as classification, regression, and representation learning. The field takes inspiration from biological neuroscience and revolves around stacking artificial neurons into layers and "training" them to process data. The adjective "deep" refers to the use of multiple layers (ranging from three to several hundred or thousands) in the network. Methods used can be supervised, semi-supervised or unsupervised.

**Large language models** (LLM): A large language model (LLM) is a machine learning model (typically a neural network) trained on a vast amount of text for natural language processing tasks, especially language generation. LLMs can typically generate, summarize, translate, and analyze text in many contexts. They are the basis for many modern chatbots, such as ChatGPT, Claude, Gemini, Grok, Qwen and DeepSeek. (https://en.wikipedia.org/wiki/Large_language_model)

---

## A01.02 · Trace the history of AI

- [x] A01.02 Trace the history of AI

> [!tip] Hint
> Turing test (1950), Dartmouth conference (1956), AI winters, expert systems, the return of neural networks, AlexNet (2012), Transformer (2017), ChatGPT (2022).

**My notes:**
From the Turing Test to ChatGPT: A Brief History of AI
1950s: The question is posed

In 1950, Alan Turing published “Computing Machinery and Intelligence,” which opened with the question “Can machines think?” Rather than define thinking, he proposed the Imitation Game, now called the Turing Test: if a human judge, chatting by text, can’t reliably tell a machine from a person, the machine should count as intelligent. The test made intelligence something you could observe in behavior, and it framed the field’s ambitions for decades.

The field got its name at the 1956 Dartmouth workshop, organized by John McCarthy, Marvin Minsky, Claude Shannon and Nathaniel Rochester. The proposal claimed that every aspect of intelligence could in principle be described precisely enough for a machine to simulate it. Early programs made that seem plausible. Newell and Simon’s Logic Theorist (1956) proved mathematical theorems, and Arthur Samuel’s checkers program learned to beat its creator. In 1958 Frank Rosenblatt’s Perceptron introduced a simple trainable artificial neuron, an early ancestor of today’s neural networks.

1960s–70s: Optimism, then the first winter

This was the era of symbolic AI, the idea that intelligence comes from manipulating symbols and rules. Joseph Weizenbaum’s ELIZA (1966) imitated a psychotherapist using simple pattern-matching. Some users became emotionally attached to it, which alarmed Weizenbaum. SHRDLU (1970) understood English commands inside a small virtual world of blocks.

The promises outran the results. In 1969 Minsky and Papert’s book Perceptrons showed that single-layer networks had serious limits, and interest in neural nets dropped. In Britain, the 1973 Lighthill Report criticized AI’s failure to scale beyond toy problems. Funding was cut on both sides of the Atlantic, starting the first AI winter in the mid-1970s.

1980s: Expert systems and the second winter

AI came back commercially through expert systems, programs that encoded specialists’ knowledge as if-then rules. Examples included MYCIN for medical diagnosis and XCON, which configured computer orders for Digital Equipment Corporation. Japan’s Fifth Generation Computer project started an international race.

Neural networks also revived. In 1986 Rumelhart, Hinton and Williams popularized backpropagation, a method for training networks with multiple layers. That answered many of the earlier objections.

Expert systems turned out to be brittle and expensive to maintain, though, and the market for specialized AI hardware collapsed. By the late 1980s and early 1990s the field was in a second AI winter.

1990s–2000s: The statistical turn

AI shifted away from hand-written rules toward learning from data, using probabilistic methods, support vector machines and Bayesian networks. Machine learning began working quietly inside spam filters, recommendation engines and speech recognition.

Several milestones reached the public:

1997: IBM’s Deep Blue beat world chess champion Garry Kasparov.
1997: Hochreiter and Schmidhuber introduced LSTM networks, which could handle sequences such as text and speech.
1998: Yann LeCun’s convolutional networks read handwritten digits on bank checks.
2011: IBM’s Watson won Jeopardy!, and Apple launched Siri.

The internet and cheap computing were also supplying two things deep learning would need: huge datasets and powerful hardware, especially GPUs.

2012–2017: The deep learning revolution

In 2012, AlexNet, built by Krizhevsky, Sutskever and Hinton, won the ImageNet image-recognition competition by a wide margin using a deep neural network trained on GPUs. Industry and academia moved to deep learning almost overnight.

Progress then came quickly:

2013: Word2Vec represented words as vectors that captured their meaning.
2014: GANs (generative adversarial networks) generated realistic images. Sequence-to-sequence models improved machine translation, and attention mechanisms were introduced.
2015: OpenAI was founded as a nonprofit research lab.
2016: DeepMind’s AlphaGo defeated Go champion Lee Sedol, a feat many experts had expected to be at least a decade away.
2017: Google researchers published “Attention Is All You Need,” which introduced the Transformer. It processes whole sequences in parallel and scales very well, and it became the architecture behind modern language models.
2018–2022: Large language models

Researchers found that training Transformers on enormous amounts of text to predict the next word produced surprisingly general abilities:

2018: OpenAI’s GPT-1 and Google’s BERT showed that pretraining on large text collections transferred well to many tasks.
2019: GPT-2 wrote fluent text. OpenAI at first held back the full model over misuse concerns.
2020: GPT-3, with 175 billion parameters, could do new tasks from just a few examples in the prompt. Work on scaling laws suggested that bigger models trained on more data improved predictably.
2021–22: DALL·E, Midjourney and Stable Diffusion brought image generation to the public, and GitHub Copilot started writing code alongside programmers.

The remaining problem was that raw language models were unpredictable and hard to steer. OpenAI’s InstructGPT (early 2022) addressed this with reinforcement learning from human feedback (RLHF): people rated the model’s responses, and the model was trained toward the answers people preferred. The result was far more helpful and better at following instructions.

November 30, 2022: ChatGPT

OpenAI released ChatGPT, a conversational interface built on GPT-3.5 and tuned with RLHF. It reached an estimated 100 million users in about two months, which made it the fastest-growing consumer app on record at the time. For the first time, millions of ordinary people were having open-ended conversations with a machine that could write essays, explain concepts, debug code and draft emails.

The thread connecting it all

The story moves in three phases:

Rules (1950s–80s): researchers tried to hand-code intelligence and found that the world is too messy for that.
Statistics (1990s–2000s): machines began learning patterns from data.
Scale (2010s onward): deep neural networks, very large datasets and massive computing power produced abilities nobody had explicitly programmed.

---

## A01.03 · Understand the three families of learning

- [x] A01.03 Understand the three families of learning

> [!tip] Hint
> Supervised (labeled data), unsupervised (hidden structure), reinforcement (rewards).

**My notes:**
## The Three Ways Machines Learn

#### 🏷️ Supervised Learning: _learning with a teacher_

The model studies **labeled examples**, where every input comes with the correct answer: emails tagged “spam” or “not spam,” photos labeled “cat” or “dog,” houses paired with their sale prices. Once it has learned the pattern, it can predict answers for data it has never seen.

> **Used in:** image recognition · medical diagnosis · fraud detection

#### 🔍 Unsupervised Learning: _finding hidden patterns_

There are **no labels** and no right answers to copy. The model explores raw data and discovers structure on its own, such as grouping customers with similar habits, flagging transactions that look unusual, or simplifying complex data.

> **Used in:** customer segmentation · anomaly detection · data compression

#### 🎮 Reinforcement Learning: _learning by trial and error_

An **agent** acts in an environment and gets **rewards** for good moves and **penalties** for bad ones. Over many attempts, it develops strategies that maximize its long-term success.

> **Used in:** AlphaGo · robotics · and, through _RLHF_, training assistants like ChatGPT

---

## A01.04 · Understand the difference between training and inference

- [x] A01.04 Understand the difference between training and inference

> [!tip] Hint
> Training builds the model, it is expensive and happens once in a while. Inference uses it, on every request.

**My notes:**
- **Training** is the first phase for an AI model. Training may involve a process of trial and error, or a process of showing the model examples of the desired inputs and outputs, or both.

- **Inference** is the process that follows AI training. The better trained a model is, and the more fine-tuned it is, the better its inferences will be — although they are never guaranteed to be perfect.

---

## A01.05 · Know what a parameter, a dataset and a model are

- [ ] A01.05 Know what a parameter, a dataset and a model are

> [!tip] Hint
> A model is a function whose parameters have been adjusted on data.

**My notes:**


---

## A01.06 · Know the major players in AI

- [ ] A01.06 Know the major players in AI

> [!tip] Hint
> Closed model labs, open source players, chip makers, cloud providers. Build your own map.

**My notes:**


---

## A01.07 · Tell apart closed models and open-weights models

- [ ] A01.07 Tell apart closed models and open-weights models

> [!tip] Hint
> What "open weights" allows, and what it doesn't tell you about the training data.

**My notes:**


---

## A01.08 · Understand why the GPU changed the game

- [ ] A01.08 Understand why the GPU changed the game

> [!tip] Hint
> Massively parallel matrix multiplication.

**My notes:**


---

## A01.09 · Watch the 3Blue1Brown Neural Networks series

- [ ] A01.09 Watch the 3Blue1Brown Neural Networks series

> [!tip] Hint
> The best visual intuition of what a neural network does.

**My notes:**


---
