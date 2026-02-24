# ProjectX-Projects-2025

This is the list of projects completed in the 2025 programme.

## Index

1. [FakeMyVoice](#fakemyvoice)
2. [Train Your Foes](#train-your-foes)
3. [Traffiq](#-traffiq)
4. [Voice2English](#voice2english)
5. [Reinforcents](#reinforcents)
6. [Neural Quest](#neural-quest)
7. [Encrypted Chat Application](#encrypted-chat-application)
8. [Text to Handwritting](#text-to-handwriting)
9. [EEG Analyser and Simulator](#eeg-analyser-and-simulator)
10. [MuseGan](#musegan)
11. [Multimodal Graph DB with RAG](#multimodal-graph-db-with-rag)
12. [CodeSage](#codesage)
13. [Sera](#sera)
14. [Kernel Design](#kernel-design)
15. [Cryptanalysis](#cryptanalysis)
16. [AI Ops](#ai-ops)

***
## FakeMyVoice
### Description
**Fake My Voice** is a deep learning-powered multi-speaker Text-to-Speech (TTS) system designed to clone voices with high fidelity. By extracting a unique **256-D speaker embedding** from just a few seconds of reference audio, the pipeline replicates the specific tone, accent, and style of any target speaker. 

The project integrates three state-of-the-art architectures:
* **GE2E Encoder:** Extracts robust vocal identity features.
* **Tacotron 2:** Generates speaker-conditioned Mel-spectrograms from text.
* **WaveGlow:** A flow-based neural vocoder for natural waveform generation.

---

### Output

### **Tacotron2 Performance**
Achieved smooth Mel-spectrogram prediction after ~60 epochs.

**Text:** *"Printing, in the only sense with which we are at present concerned"*

| Expected Mel | Predicted Mel | Predicted Frames |
| :---: | :---: | :---: |
| ![Expected mel](https://raw.githubusercontent.com/nihira20/Fake_My_Voice/main/images/target_mel.png) | ![mel predicted](https://raw.githubusercontent.com/nihira20/Fake_My_Voice/main/images/mel_64.png) | ![output frames](https://raw.githubusercontent.com/nihira20/Fake_My_Voice/main/images/output_frames.png) |

### **Speaker Embeddings**
Achieved stable separation across 40+ speakers. t-SNE plots show distinct identity clustering.

<p align="center">
  <img src="https://raw.githubusercontent.com/nihira20/Fake_My_Voice/main/images/embeddings.jpg" width="400">
</p>

### **Losses & Metrics**
- **Mel Prediction:** Mean Squared Error (MSE) Loss.
- **Stop Token:** Binary Cross-Entropy (BCE) Loss.
<p align="center">
  <img src="https://raw.githubusercontent.com/nihira20/Fake_My_Voice/main/images/loss.png" width="400">
</p>

### **Audio Output**
[Download/Listen to Audio Sample](https://raw.githubusercontent.com/nihira20/Fake_My_Voice/main/images/model_output_fmv.wav)

> *The audio says : "Use this model to clone the voice of any user"*

---

### References
* **Source Code:** [FakeMyVoice-Project-X-2025](https://github.com/nihira20/Fake_My_Voice)
* **Research Papers:** [Tacotron 2](https://arxiv.org/pdf/1712.05884), [GE2E Loss](https://arxiv.org/pdf/1710.10467), [WaveGlow](https://arxiv.org/pdf/1811.00002).
* **Datasets:** LJSpeech, VoxCeleb, and VCTK Corpus.
* **Implementation:** [NVIDIA Tacotron 2 + WaveGlow](https://github.com/NVIDIA/tacotron2)

**Mentors:**
* Kevin Shah
* Prasanna Kasar
* Yash Ogale

**Domains:** Deep Learning, Speech & Audio Signal Processing, Natural Language Processing (TTS)

***
## Train Your Foes
### Description
<p align="justify">
  <strong>Train Your Foes</strong> is a game where your greatest enemy is a machine that learns from you. Built in <strong>Unity 6</strong>, the game is split into two parts. First, you face <strong>The Gauntlet</strong>: four intense platforming levels that test your speed and precision. If you survive, you enter <strong>The Duel</strong>: a final boss fight that isn't scripted. Instead of following a set pattern, the boss uses <strong>Artificial Intelligence (Q-Learning)</strong> to study your health, energy, and moves. It chooses the best strategy to defeat you based on thousands of past battles, creating a unique challenge that feels alive and unpredictable.
</p>

### Output images
<p align="center">
  <img width="512" height="447" alt="image" src="https://github.com/user-attachments/assets/386176d2-7cd4-4d94-80bb-2f7acb1e0ef4" />
  <img width="960" height="537" alt="image" src="https://github.com/user-attachments/assets/df901011-a56f-4277-806a-a0701131565a" />
</p>

### References
<p align="justify">
  1. <strong>Documentation:</strong> <a href="https://avanishsalunke.github.io/TRAIN-YOUR-FOES/">Full Documentation Site</a><br>
  2. <strong>Source Code:</strong> <a href="https://github.com/AvanishSalunke/TRAIN-YOUR-FOES/">GitHub Repository</a><br>
  3. <strong>Engine:</strong> Unity Engine (<code>6000.2.1f1</code>)<br>
  4. <strong>Algorithm:</strong> Custom Q-Learning Implementation using the Bellman Equation:
</p>

$$Q(s, a) \leftarrow Q(s, a) + \alpha [R + \gamma \max_{a'} Q(s', a') - Q(s, a)]$$

**Mentors:**
<p align="justify">
  • <a href="https://github.com/Abhay-Varnekar"><strong>Abhay Varnekar</strong></a><br>
  • <a href="https://github.com/Ishaan0132"><strong>Ishaan Shaikh</strong></a>
</p>

**Domains:** Game Development, Artificial Intelligence, Reinforcement Learning

***

## 🚦 Traffiq
### Description
<p align="justify">
<strong>TrafIQ</strong> is an intelligent traffic signal control system that uses <strong>Deep Reinforcement Learning (DRL)</strong> to optimize signal timings in real-time. Built using <strong>SUMO</strong> simulation and algorithms such as <strong>Q-Learning, DQN, PPO, and MAPPO</strong>, the system dynamically adapts to traffic conditions to reduce queue lengths, waiting time, and emissions while maximizing throughput.
</p>

### Output images
<p align="center">
  <img src="https://raw.githubusercontent.com/sofiaabidi/TraffIQ-Project-X-2025/main/results/visualizations/sumo.png" height="260"/>
  <img src="https://raw.githubusercontent.com/sofiaabidi/TraffIQ-Project-X-2025/main/results/single_intersection/ppo/queue_length.png" height="260"/>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/sofiaabidi/TraffIQ-Project-X-2025/main/results/visualizations/image.png" width="75%"/>
</p>

### References
<p align="justify">
1. <strong>Documentation:</strong> <a href="https://sofiaabidi.github.io/TraffIQ-Project-X-2025/">Project Documentation</a><br>
2. <strong>Source Code:</strong> <a href="https://github.com/sofiaabidi/TraffIQ-Project-X-2025">GitHub Repository</a><br>
3. <strong>Simulation Engine:</strong> SUMO (Simulation of Urban Mobility)<br>
4. <strong>Frameworks:</strong> PyTorch, Gymnasium
</p>

**Mentors:**
- Yashvi Mehta  
- Mahi Palimkar  

**Domains:** Reinforcement Learning, Multi-Agent Systems, Intelligent Transportation Systems  

***

## Voice2English
### Description

### Output images

### References

**Mentors:**

**Domains:**

***

## Reinforcents
### Description

### Output images

### References

**Mentors:**

**Domains:**

***

## Neural Quest
### Description

### Output images

### References

**Mentors:**

**Domains:**

***
## Encrypted Chat Application
### Description
<p align="justify">
  <strong>Cryptify </strong> is a secure real-time messaging system built using <strong>Java Socket Programming</strong> and <strong>Spring Boot</strong>, designed to demonstrate low-level encrypted communication over TCP. The application implements <strong>Hybrid Cryptography</strong>, combining <strong>RSA (for secure key exchange)</strong> and <strong>AES (for fast symmetric message encryption)</strong> to ensure confidentiality and integrity. Messages are encrypted before transmission, securely exchanged over TCP sockets, and decrypted only by the intended recipient, ensuring that no plain-text data is exposed during communication.
</p>

### Output images
<p align="center">
<img width="1851" height="1056" alt="image" src="https://github.com/user-attachments/assets/6cbdab2f-a3fa-4663-8933-f7162fb53e2a" />

 <img width="1852" height="1056" alt="image" src="https://github.com/user-attachments/assets/3168380c-0a05-4e97-8fdd-ec26def10b46" />

### References
<p align="justify">
  1. <strong>Source Code:</strong> <a href="https://github.com/MohdHedayati/Encrypted-Chat-Application">GitHub Repository</a><br>
2. <strong>Documentation:</strong> <a href="https://mohdhedayati.github.io/Encrypted-Chat-Application/">Project Documentation</a><br>
3. <strong>Encryption Standard:</strong> RSA-2048 for key exchange<br>
4. <strong>Symmetric Encryption:</strong> AES-256 (GCM mode recommended)<br>
5. <strong>Transport Protocol:</strong> TCP Socket Programming in Java<br>
6. <strong>Security Model:</strong> Hybrid Encryption (RSA + AES)
</p>

**Mentors:**
<p align="justify">
  • <a href="https://github.com/aitwehrrg"><strong>Rupak Gupta</strong></a><br>
  • <a href="https://github.com/Tanish2207"><strong>Tanish Bhamare</strong></a>
</p>

**Domains:** Cybersecurity, Network Programming, Cryptography, Secure Communication

***

## Text to Handwriting

### Description
This project generates realistic handwritten text from typed input using a Conditional Generative Adversarial Network (CGAN).  
Unlike traditional handwriting synthesis systems that require large datasets or fixed vocabularies, this model learns writer-specific style from a small set of handwriting samples (approximately 15 images per writer).

A Content Encoder preserves textual correctness, while a Style Encoder captures unique handwriting characteristics. The Generator combines both representations to produce natural-looking handwritten word images.

### Output Images
The system produces handwritten word images that reflect:
- The provided input text  
- Writer-specific stylistic features  
- Natural handwriting variations  

![alt text](https://raw.github.com/hredayshah2507/Text-To-Handwriting/main/image-1.png)

![alt text](https://raw.github.com/hredayshah2507/Text-To-Handwriting/main/image-9.png)

![alt text](https://raw.github.com/hredayshah2507/Text-To-Handwriting/main/image-10.png)

![alt text](https://raw.github.com/hredayshah2507/Text-To-Handwriting/main/image-11.png)

![alt text](https://raw.github.com/hredayshah2507/Text-To-Handwriting/main/image-12.png)

### References
- GANwriting: Content-Conditioned Generation of Styled Handwritten Word Images  
- IAM Handwriting Word Database  
- Deep Learning Specialization — DeepLearning.AI  
- Kaggle Datasets  

**Mentors:**  
- [Kavya Rambhia](https://github.com/kavya-r30)
- [Viraj Vora](https://github.com/viraj200524) 

**Domains:** Computer Vision, Generative Adversarial Networks (GANs), Natural Language Processing  

***

## EEG Analyser and Simulator
### Description
<p align="justify">
  <strong>EEG Analyser and Simulator</strong> is a AI-driven simulation and prediction of brain dynamics using EEG data. This project aims to develop an AI-powered system that constructs a personalized Digital Twin of the Brain using EEG (Electroencephalogram) data.
The system leverages deep learning and signal processing to analyze, predict, and simulate neurological patterns — enabling early detection of epilepsy, cognitive stress, depression, and other brain-related conditions. The system also aims to classify emotions in awake and dream phase. Other implications include the prediction of failure and success of surgery and drug identification and simulation of its effects on EEG data.
In addition, the project explores neural generative modeling to interpret REM-phase brain activity into abstract visual representations, pushing the boundaries of dream analysis and subconscious understanding.
</p>

### Output images

The system predicts the desired label for EEG signal and also plots it.

![alt_text](https://raw.githubusercontent.com/ajatshatru01/EEG-Analyser-and-simulator/main/EEG_Analyser/docs/output1.jpeg)

![alt text](https://raw.githubusercontent.com/ajatshatru01/EEG-Analyser-and-simulator/main/EEG_Analyser/docs/output2.jpeg)

![alt text](https://raw.githubusercontent.com/ajatshatru01/EEG-Analyser-and-simulator/main/EEG_Analyser/docs/output3.jpeg)

### References
- [Transformer paper](https://arxiv.org/abs/1706.03762)
- Datasets:- SEED, TUH HUP, HUP iEEG, SAM40, DEED
- [LSTM](https://arxiv.org/html/2408.10328v1)
- [EEG SIGNAL PROCESSING](https://mne.tools/stable/auto_tutorials/intro/10_overview.html)
  
**Mentors:**
- [Ghruank Kothare](https://github.com/Ghruank)
- [Afreen Kazi](https://github.com/Afreen-Kazi-1)
  
**Domains:** Signal processing, Machine Learning, Deep Learning

***

## MuseGan

### Description
MuseGan is a GAN-based project for generating multi-track polyphonic music. It can generate coherent 4-bar music for 5 instruments from scratch and also supports Human-AI collaboration by conditionally generating tracks based on one human input track.

### Output images

#### From-Scratch Model
<p align="center">
  <img src="https://github.com/user-attachments/assets/27d00a7c-5d2f-4d82-a1fa-c59f3949e5d8" alt="Model Diagram" width="600"/>
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/b926765e-d4f7-49e5-a967-e3168d6676db" alt="Pianoroll Output" width="600"/>
</p>

#### Conditional Track
<p align="center">
  <img src="https://github.com/user-attachments/assets/084d9045-3254-47cf-ad04-376a9f79c8ac" alt="Conditional Model Diagram" width="600"/>
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/02bcc0b9-4b67-447f-af9f-041067b28a8b" alt="Conditional Outputs" width="600"/>
</p>

### References
- Documentation: [MuseGAN](https://sonu0305.github.io/MuseGAN-docs/) 
- MuseGAN README: [MuseGAN.md](./MuseGAN.md)
- MuseGAN Repository: [MuseGAN Repository](https://github.com/Star-Light-9/MuseGAN)

**Mentors:**
- [Kavya Rambhia](https://github.com/kavya-r30)  
- [Swayam Shah](https://github.com/sonu0305)

**Domains:** Music Generation, Generative Adversarial Networks (GANs), Temporal Sequence Modeling  

***

## Multimodal Graph DB with RAG
### Description

### Output images

### References

**Mentors:**

**Domains:**

***

## CodeSage
### Description

**CodeSage** is a Python-based framework that executes code and explains its logic in simple, human-readable language.  
It combines compiler concepts with AI-based summarization to help users understand how code works internally.

### Pipeline
- **Lexer** → Converts source code into tokens  
- **Parser** → Builds an Abstract Syntax Tree (AST)  
- **Summarizer** → Generates structured explanations  
- **Interpreter** → Executes the AST (tree-walk)  
- **NLP (Optional)** → Refines explanations  
- **GUI (Tkinter)** → Editor, output, AST view, summaries  

### Purpose
- Help students understand how interpreters work  
- Explain code behavior clearly  
- Visualize program structure  
- Bridge programming with AI-based explanation  

**CodeSage runs code and explains it step-by-step.**

### Output images
<img width="877" height="518" alt="image" src="https://github.com/user-attachments/assets/2bda37c8-5d7c-4d7a-917f-7691f3930c7c" />
<img width="895" height="651" alt="image" src="https://github.com/user-attachments/assets/ac11c585-089e-416a-92a2-8de5f8919fdd" />


### References
- https://github.com/Mokshii46/CODESAGE
- https://Mokshii46.github.io/CODESAGE/

**Mentors**: Yadnyesh Patil, Rupak Gupta

**Domains**: AST Parsing NLP

***

## Sera
### Description

### Output images

### References

**Mentors:**

**Domains:**

***

## Kernel Design
### Description

### Output images

### References

**Mentors:**

**Domains:**

***

## Cryptanalysis
### Description
Cryptanalysis is a hybrid framework combining energy-based learning, side-channel analysis, and classical cryptography to analyze multiple ciphers. It first detects the cipher (AES, DES, Speck, or Vigenère), then applies an appropriate side-channel attack method with CNN-based key recovery for DES and Speck, statistical techniques for Vigenère, and only detection for AES due to its robustness. The system highlights how different ciphers require distinct attack strategies and demonstrates both practical vulnerabilities and modern security limits.
   
### Output images
<img width="1865" height="1144" alt="DES_sca" src="https://github.com/user-attachments/assets/1f6ed8d9-6b5a-4aa9-9e33-ca41352b7ac1" />
<img width="1860" height="937" alt="speck32_sca" src="https://github.com/user-attachments/assets/9c18ab9f-8508-4076-822d-809fa6639938" />
<img width="801" height="469" alt="energy_classifier_accuracy" src="https://github.com/user-attachments/assets/eda966e2-7aa5-4820-956c-1f5071967215" />
<img width="821" height="474" alt="vignere_final_loss - 2" src="https://github.com/user-attachments/assets/5f6827f6-14f3-4619-bfc1-c5a1dd8d8783" />

### References
- [Repository Link](https://github.com/AnuushkaY/EnergyBased-and-Neurosymbolic-Methods-for-Advanced-CrypytAnalysis)  
- [Documentation Link](https://anuushkay.github.io/Cryptanalysis_Documentation/)
  
**Mentors:**
- [Afreen Kazi](https://github.com/Afreen-Kazi-1)  
- [Ghruank Kothare](https://github.com/Ghruank)
  
**Domains:** Side Channel Analysis, Energy-Based Models, Deep Learning, Cybersecurity, Classical Cryptography 

***

## AI Ops
### Description

### Output images

### References

**Mentors:**

**Domains:** 

***
