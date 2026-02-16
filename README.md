# ProjectX-Projects-2025

This is the list of projects completed in the 2025 programme.

## Index

1. [FakeMyVoice](#fakemyvoice)
2. [Train Your Foes](#train-your-foes)
3. [Traffiq](#traffiq)
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

### Output images

### References

**Mentors:**

**Domains:**

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

## Traffiq
### Description

### Output images

### References

**Mentors:**

**Domains:**

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

### Output images

### References

**Mentors:**

**Domains:**

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
- [VirajVora](https://github.com/viraj200524) 

**Domains:** Computer Vision, Generative Adversarial Networks (GANs), Natural Language Processing  

***

## EEG Analyser and Simulator
### Description

### Output images

### References

**Mentors:**

**Domains:**

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

### Output images

### References

**Mentors:**

**Domains:**

***

## AI Ops
### Description

### Output images

### References

**Mentors:**

**Domains:**

***
