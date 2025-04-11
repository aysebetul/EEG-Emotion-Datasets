# EEG-Emotion-Datasets
List of publicly available EEG-emotion datasets. 
You can load some of these datasets via [torcheeg datasets](https://torcheeg.readthedocs.io/en/v1.0.11/torcheeg.datasets.html)

1. [DEAP](https://www.eecs.qmul.ac.uk/mmv/datasets/deap/): \
   [Paper](https://ieeexplore.ieee.org/document/5871728) - DEAP: A Database for Emotion Analysis ;Using Physiological Signals (2012) \
   **EEG Data:** 32 participants, 32 channels, 40 music videos, 40 trials \
   **Device:** Biosemi (10-20 system) \
   **Recordings:** 48 recorded channels (32 EEG channels, 12 peripheral channels, 3 unused channels, and 1 status channel) at 512Hz. (Downsampled to 128 Hz) \
   **Stimuli:** One-minute music video clips(not instrumental) rated by 14-16 volunteers based on arousal, valence, and dominance. (selected 40 out of 120 video clips) \
   [happy stimuli](https://www.youtube.com/watch?v=QvD6maGRh7c) \
   [sad stiumli](https://www.youtube.com/watch?v=cQHJuSZTjkE) \
   [angry stimuli](https://www.youtube.com/watch?v=ZxcCN6BgO_k) \
   **Labels:** Obtained using Self-Assessment Manikin (discrete scores 1-9) for each dimension  valence, arousal, dominance, liking 
   
2. [SEED](https://bcmi.sjtu.edu.cn/home/seed/seed.html): \
   **EEG Data:** 15 participants, 62 channels, 3 sessions, 15 film clips, 15 trials \
   **Device:** 62-channel ESI NeuroScan System (10-20 system) \
   **Recordings:** The EEG data was downsampled to 200 Hz and applied  bandpass filter between 1 Hz and 75 Hz. EEG signals and eye movements were collected with the 62-channel ESI NeuroScan System and SMI eye-tracking glasses \
   **Stimuli:** 15 Chinese film clips (approximately 4 minutes) (happiness, sadness, fear, neutral emotions) \
   **Labels:** Self Assessment via questionnaire, happiness, sadness, fear, neutral emotions 
   
3. [SEED-IV](https://bcmi.sjtu.edu.cn/home/seed/seed-iv.html): \
   **EEG Data:** 15 participants, 62 channels, 3 sessions, 72 film clips, 24 trials \
   **Device:** 62-channel ESI NeuroScan System (10-20 system) \
   **Recordings:** The EEG data was downsampled to 200 Hz and applied  bandpass filter between 1 Hz and 75 Hz. EEG signals and eye movements were collected with the 62-channel ESI NeuroScan System and SMI eye-tracking glasses \
   **Stimuli:** 15 Chinese film clips (approximately 4 minutes) (positive, neutral and negative emotions) \
   **Labels:** Self Assessment via questionnaire, positive(1), negative(-1), and neutral(0) 
   
4. [DENS](https://openneuro.org/datasets/ds003751/versions/1.0.2): Dataset on Emotion with Naturalistic Stimuli \
   [Paper](https://www.biorxiv.org/content/10.1101/2021.08.04.455041v2.full) - Dataset on Emotion with Naturalistic Stimuli (DENS) on Indian Samples (2022) \
   **EEG Data:** 40 participants, 128 channels, \
   **Device:** 128 electrode system from EGI Inc. (10-10 system) \
   **Recordings:**  EEG, ECG, EMG. EEG data is bandpass filtered from 1-40 Hz. and the sampling rate is 250 Hz. \
   **Stimuli:** 16 emotional stimuli were selected from the affective multimedia stimuli dataset validated on Indian samples. The time duration for each stimulus is 60 seconds. 
   Stimuli Emotion labels - Adventurous, Afraid, Alarmed, Amused, Angry, Aroused, Calm, Disgust, Enthusiastic, Excited, Happy, Joyous, Melancholic, Miserable, Sad, and Triumphant. \
   **Labels:** Self-assessment (discrete scores 1-9 ) for Valence, Arousal, Dominance. (discrete scores 1-5) for Liking, Familiarity. A continuous scale of 1 to 5 for Relevance. Emotion category 
   
5. [EEG Dataset for the Recognition of Different Emotions Induced in Voice-User Interaction](https://springernature.figshare.com/articles/dataset/Preprocessed_Dataset/25751097?backTo=/collections/EEG_Dataset_for_the_Recognition_of_Different_Emotions_Naturally_Induced_in_Voice-User_Interaction/7207839) \
   [Paper](https://www.nature.com/articles/s41597-024-03887-9#Sec9) EEG Dataset for the Recognition of Different Emotions Induced in Voice-User Interaction (2024) \
   **Data:** 44 participants, 63 channels, 80 trials \
   **Device:** ActiChamp EEG Amplifier (Brain Products) (10-10 system) \
   **Recordings:** EEG, ECG, PPG, GSR, and facial expression. They applied a notch filter (59-61Hz) and a bandpass filter(1-80Hz). Subsequently, EEG signal is downsampled from 1000Hz to 200 Hz. The preprocessed data is segmented for the "answer period" since they investigate the emotion change in response to the answer of VUI and emotion would be mostly induced in this period. \
   **Stimuli:** They aimed to create voice stimuli using a Voice User Interface(VUI) system that mimics natural human-to-human communication. Two parameters are controlled in the VUI system, voice type(child/adult) and information quantity(simple/detailed). User satisfaction with the answers provided by VUI is considered as ground truth for induced emotion. They prepared 80 questions and answers. During the experiment, participants ask the question to VUI by reading the question and the answer is given from among four types (child/simple, child/detailed, adult/simple, adult/detailed). \
   **Labels:** Participant defines the emotion based on some criteria such as interesting, obvious, impressive, etc. (each score -3 to 3) 
   
6. [EAV](https://github.com/nubcico/EAV) \
   [Paper](https://www.nature.com/articles/s41597-024-03838-4) - EAV: EEG-Audio-Video Dataset for Emotion Recognition in Conversational Contexts (2024) \
   **Data:** 42 participants, 30 channels, 200 interactions \
   **Device:** 30 channels BrainAmp System (Brain Products) \
   **Recordings:** EEG, audio, video. EEG data was recorded at a rate of 500 Hz. Additionally, they applied a high-pass filter (0.5 Hz) and bandpass filter(50 Hz). Data is segmented into 20-second epochs. \
   **Stimuli:** In the experiments, participants are engaged in emotional dialogues with a conversational system. Therefore, dialogues have multiple iterations of "speaking" and "listening". Dialogues are generated by ChatGPT and edited by humans to ensure emotional clarity. \ Participants watch the pre-recorded video (listening interaction) and then respond to the corresponding dialogue by reading from the monitor (speaking interaction). Each participant is included in 100 repeated interactions. Visual stimuli and dialogues are displayed during the experiment. \
   **Labels:** Five distinct emotions - neutral, anger, happiness, sadness and calmness. Participants selected five dialogues (each has 4 interactions) for each emotional class so that class labels are established before the experiment. They also did self-assessment to indicate their perceived emotion with arousal and valence score (-5 to 5) after each iteration. 
   
7. [MPED](https://github.com/Tengfei000/MPED/tree/datatset) \
   [Paper](https://ieeexplore.ieee.org/document/8606087) - MPED: A Multi-Modal Physiological Emotion Database for Discrete Emotion (2019) \
   **Data:** 23 participants, 62 channels, 14 trials, 28 videos \
   **Device:** 62 channel ESI NeuroScan System (10-20 system) \
   **Recordings:** EEG, ECG, Galvanic skin response, respiration. The EEG sampling rate is 1000 Hz. \
   **Stimuli:** Video clips. Video clips are selected after detailed experiments and assessed by three psychological questionnaires (PANAS, SAM, DES). \
   **Labels:** 7 discrete emotions. (neutral, joy, funny, disgust, anger, fear, sad). Additionally, after the experiment, participants conducted self-assessments. 
    
8. [DREAMER](https://zenodo.org/records/546113) \
   [Paper](https://ieeexplore.ieee.org/document/7887697) - DREAMER: A Database for Emotion Recognition Through EEG and ECG Signals From Wireless Low-cost Off-the-Shelf Devices (2018) \
   **Data:** 23 participants, 16 channels, 18 film clips \
   **Device:** Emotiv EPOC wireless EEG headset (10-20 system) \
   **Recordings:** EEG and ECG. The EEG sampling rate is 128 Hz. The Artefact Subspace Reconstruction method is used to remove artifacts. \
   **Stimuli:** Audio and visual stimuli of film clips targeted 9 emotions (amusement, excitement, happiness, calmness, anger, disgust, fear, sadness, and surprise) \
   **Labels:** Self-assessment in terms of arousal, valence, and dominance (scores 1-5) 
   
9. [AMIGOSDataset](https://www.eecs.qmul.ac.uk/mmv/datasets/amigos/index.html) \
   [Paper](https://ieeexplore.ieee.org/document/8554112) - AMIGOS: A Dataset for Affect, Personality and Mood Research on Individuals and Groups (2021) \
   **Data:** Short video experiment: 40 participants, 14 channels, 16 videos, 16 trials \
   Long video experiment (individual): 17 participants, 14 channels, 4 videos, 2 trials \
   Long video experiment (group): 20 participants, 14 channels, 4 videos, 2 trials \
   **Device:** Emotiv EPOC Neuroheadset \
   **Recordings:** EEG, ECG, GSR, frontal HD video of participants. EEG data is recorded at a rate of 128 Hz, signals are average-referenced, and a high-pass filter (2Hz) is applied. \
   **Stimuli:** 16 short videos and 4 long videos. 2 experiments: In the first one 40 participants watched 16 short emotional videos and in the second experiment, participants watched 4 long videos (some of them alone and the rest in groups) Stimulus are annotated on valence and arousal dimension. \
   **Labels:** Self assessment of affective levels (valence(1-9), arousal(1-9), control(1-9), familiarity(1-9), liking(1-9) and basic emotions(neutral, happiness, sadness, surprise, fear, anger, disgust)) 
   
10. [PEGCONV](https://pegconv.nastaran-saffar.me) \
    [Paper](https://dl.acm.org/doi/10.1145/3490099.3511148) - Emotion Recognition in Conversations Using Brain and Physiological Signals (2022) \
    **Data:** 23 participants, 16 channels \
    **Device:** All-in-One EEG Electrode Cap Starter Kit with cyton-daisy board from OpenBCI (Wireless) (10-20 system) \
    **Recordings:** EEG, audio, video, GSR, PPG. EEG data was recorded at the rate of 125 Hz. \
    **Stimuli:** Questions asked by the interviewer (pre-intern psychologist) to induce the targeted emotion. \
    **Labels:** Five emotions: happiness, sadness, anger, fear, neutral state. Participants listened to the conversations and labeled their emotions using self-report questionnaires (scores 1-5). Each trial was divided into three parts (beginning, in the middle, at the end), and collected three emotions for each trial. 
    
11. [INTERFACES datasets](https://github.com/IoBT-VISTEC/EEG-Emotion-Recognition-INTERFACES-datasets) \
    [Paper](https://ieeexplore.ieee.org/document/8762012) - Consumer Grade Brain Sensing for Emotion Recognition (2019) \
    **Data:** 43 participants, 15 videos, 8 channels \
    **Device:** OpenBCI (10-20 system) \
    **Recordings:** EEG, EDA, BVP, Temp. EEG data is recorded at the rate of 250 Hz. \
    **Stimuli:** Movie clips from IMDb. Selected video clips are eliminated with affective video selection experiment. Participants of this experiment assessed their emotions in terms of valence, arousal, happiness, fear, and excitement. (each on scale 1-9) \
    **Labels:** Self-emotional assessment in valence, arousal, happiness, fear, and excitement. (each on scale 1-9) 
    
