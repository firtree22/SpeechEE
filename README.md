# SpeechEE: A Novel Benchmark for Speech Event Extraction

Bin Wang<sup>1</sup>, Meishan Zhang<sup>1</sup>, Hao Fei<sup>2, *</sup>, Yu Zhao<sup>3</sup>, Bobo Li<sup>4</sup>, Shengqiong Wu<sup>2</sup>, Wei Ji<sup>2</sup>, Min Zhang<sup>1</sup>

<sup>1</sup>Harbin Institute of Technology (Shenzhen)
<sup>2</sup>National University of Singapore  
<sup>3</sup>Tianjin University 
<sup>4</sup>Wuhan University  


Accepted by ACM MM 2024 (Poster)  
(* Correspondence)



## Abstract

Event extraction (EE) is a critical direction in the field of information extraction, laying an important foundation for the construction of structured knowledge bases.
EE from text has received ample research and attention for years, yet there can be numerous real-world applications that require direct information acquisition from speech signals, online meeting minutes, interview summaries, press releases, etc.
While EE from speech has remained under-explored, this paper fills the gap by pioneering a \textbf{SpeechEE}, defined as detecting the event predicates and arguments from a given audio speech.
To benchmark the SpeechEE task, we first construct a large-scale high-quality dataset.
Based on textual EE datasets under the sentence, document, and dialogue scenarios, we convert texts into speeches through both manual real-person narration and automatic synthesis, empowering the data with diverse scenarios, languages, domains, ambiences, and speaker styles.
Further, to effectively address the key challenges in the task, we tailor an E2E SpeechEE system based on the encoder-decoder architecture, where a novel Shrinking Unit module and a retrieval-aided decoding mechanism are devised.
Extensive experimental results on all SpeechEE subsets demonstrate the efficacy of the proposed model, offering a strong baseline for the task. 
At last, being the first work on this topic, we shed light on key directions for future research.


To be continued ...


