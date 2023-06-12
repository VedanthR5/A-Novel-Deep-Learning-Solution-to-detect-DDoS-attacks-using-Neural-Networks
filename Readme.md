<a name="br1"></a> 

**A Novel Supervised Deep Learning Solution to detect Distributed Denial of Service (DDoS) attacks on Edge**

**Systems using Convolutional Neural Networks (CNN)**

***Note: Figures are created from cited***

**SCIENTEER PROJECT ID: 182334**

***sources or are my own***

**1: Background and Rationale**

**5b: Results**

**4a: Proce**

• Therefore, models to

\- **The proposed model was tested on over 5000 samples of**

**unseen DDoS flows.**

\- The Confusion Matrix below shows that our model was very

successful. We can use these values to analyze our results in the

form of other common performance metrics

• The growing foray of

Distributed Denial of Service

(DDoS) attacks has caused the

unavailability of millions of

cloud services,

• Up to $660 Billion in loss of

revenue (1),

**1. Data Preprocessing Algorithm**

In order to analyze the dataset and implement our

CNN model, we had to preprocess our data to

ensure the fairness and equality of the spread of

data to get the most accurate results.

• Algorithm 1 uses key feature extraction to

parse packets into “flows” and time stamps

(headers and columns) to easily feed into

the CNN Model.

1\. The output of the preprocessing algorithm (Fig. 5) will

then input the proposed CNN Architecture to be trained.

(Figure 6)

defend and mitigate DDoS

traffic need to have three

features.

• Scalability, Flexibility,

Reliability

\- True Negative (TNR), True Positive (TPR)

\- False Negative (FNR), False Positive (FPR)

• Current state of the art

models, lack at least one

of these components.

• The model **proposed will**

**have to include these 3**

**features** and use machine

learning to build an active

intrusion detective

• DDoS is a threat to basic

internet standards and security.

• DDoS attacks critical services

and flood the network with

malicious traffic.

**Fig. 7. Confusion Matrix of Testing**

**accuracy of CNN Model**

• Normalize and pad the resultant flow of

data

**Fig. 3. Proposed CNN architecture training flow**

• In the first half of 2022 alone,

there were 6,019,888 DDoS

attack devices across the

world. (2)

2\. A 2D convolutional layer with 64 filters and a kernel size of 3 x 3.

• The convolutional layer will be responsible

for extracting features from the input data by

sliding the filters over the input and

system (IDS)

computing dot products  (9).

(푻푷푹+푻푵푹)

**Accuracy:**

= ퟗퟕ. ퟕ%

**Rationale:** Create a novel

supervised model, that

can handle any size of

data and differentiate

between malicious and

benign traffic consistently.

This model should be

functional on private and

(푻푷푹+푻푵푹+푭푷푹+푭푵푹)

(푻푷+푻푵)

3\. A dropout layer with a recommended

*dropout rate of 0.5 (11).*

• This layer will randomly set a certain

percentage of input units to 0 at each update

during training time, which helps prevent

overfitting.

**F1 Score:**

= ퟗퟕ. ퟐ%

푻푷+푻푵+푭푷+푭푵

**6: Discussion /Conclusions**

**~~Strengths of this study:~~**

• Here we will use the ReLU (Rectified Linear

Unit)  activation function. This function

calculates the output of a neuron as the

maximum between 0 and the input value,

• Automated hyperparameter setup to fine tune and

optimized to not keep lower accuracy model

• The model’s use of validation-test split optimizes

the model for different features in PCAP files

• The ReLU Activation and kernel technique was able

to successfully identify the importance of specific

features with respect to others.

o **~~Further Research~~**

**Fig. 1: Attacker to User network connectivity**

public networks

**Fig. 4. Flow Chart illustrating the**

**algorithm**

mathematically represented as

**2a: Engineering Question**

푓 푥 = max 0,1

• Turns off neurons that do not affect the

prediction

4\. A GlobalMaxPooling2D layer. This layer will

perform max pooling on the input, which

reduces the spatial dimensions of the input

**Fig. 2: Algorithm with DDoS data preprocessing in Python**

Can a dynamic deep learning model effectively differentiate

between malicious and benign traffic based on different

characteristics of the dataset? Additionally, can CNN models be

successfully applied to the field of cybersecurity?

**2. CNN Model Architecture**

Next, we implemented our CNN model using TensorFlow and

• The model is based on a lab- based

environment and dataset

• However, the algorithm can be

trained for more complicated

circumstances

• Can be developed into an active IDS

platform to implement in the real

the Keras API for ease of coding and debugging. (See 4b. CNN while retaining important features.

5\. A flattened layer. This layer will flatten the

output of the previous layer into a one-

dimensional tensor.

6\. The final fully connected layer will

contain a **sigmoid activation function**

(Figure 6) (12).

Architecture)

**2b. Engineering Goal**

**3. Training**

Finally, we will use the Adam optimizer for training the model

and set the learning rate, batch size, and number of epochs as

hyperparameters that the model tunes each iteration.

The engineering goal of this project is to **~~design and develop a~~**

**~~dynamic deep learning model that can accurately identify~~**

**~~malicious and benign network traffic~~**  across a wide range of

attack methods and situations, even when dealing with large

amounts of real-time data in short time constraints.

1

**Fig. 5. Probability of a DDoS attack**

**(in the fully connected layer as**

**a function of the input data set)**

휙 푧 =

The data will be evenly split into 3 distinct sets (train, test, val)

in HDF5 format for readability

−푧

world

1 + ⅇ

•

This layer will perform the final computation

to output a probability of the input being a

DDoS attack.

**6: Bibliography**

**4. Testing**

**3: Dataset and Materials**

The model will be tested under common performance metrics

such as a confusion matrix, accuracy, and F1 Score (See 5.

Results for more information)

• Outputs a number between 0 and 1 as labels

to designate benign vs malicious traffic

• When *p* > .5, the attack will be classified as a

DDoS attack, otherwise it is benign.

1\. AO Kaspersky Lab. (2023, January 10). Distributed denial of service: Anatomy and impact of DDoS attacks.

www.kaspersky.com. Retrieved January 22, 2023, from https://www.kaspersky.com/resource-center/preemptive-

safety/how-does-ddos-attack-work

2\. NetScout. (2022, September 26). NETSCOUT DDoS Threat Intelligence Report - Latest Cyber Threat Intelligence

Report. Netscout. Retrieved January 18, 2023, from https://www.netscout.com/threatreport/

3\. What is DDoS mitigation? [Internet]. Cloudflare. Cloudflare Inc.; 2019 [cited 2022Dec22]. Available from:

https://www.cloudflare.com/learning/ddos/ddos-mitigation/

4\. Kawtar Bouzoubba, Youssef Taher, and Benayad Nsiri, “Predicting DOS-DDOS Attacks: Review and Evaluation Study

of Feature Selection Methods based on Wrapper Process”.International Journal of Advanced Computer Science and

Applications(IJACSA), 12(5), 2021. http://dx.doi.org/10.14569/IJACSA.2021.0120517

5\. Mahjabin T, Xiao Y, Sun G, Jiang W. “A survey of distributed denial-of-service attack, prevention, and mitigation

techniques.” International Journal of Distributed Sensor Networks. 2017;13(12). doi:10.1177/1550147717741463

6\. S. T. Zargar, J. Joshi and D. Tipper, "A Survey of Defense Mechanisms Against Distributed Denial of Service (DDoS)

Flooding Attacks," in IEEE Communications Surveys & Tutorials, vol. 15, no. 4, pp. 2046-2069, Fourth Quarter 2013,

doi: 10.1109/SURV.2013.031413.00127.

7\. T. Kim, B. Kang, M. Rho, S. Sezer, and E. G. Im, “A multimodal deep learning method for android malware detection

using various features,” IEEE Transactions on Information Forensics and Security, vol. 14, no. 3, pp. 773–788, March

2019\.

8\. Iman Sharafaldin, Arash Habibi Lashkari, Saqib Hakak, and Ali A. Ghorbani, "Developing Realistic Distributed Denial

of Service (DDoS) Attack Dataset and Taxonomy", IEEE 53rd International Carnahan Conference on Security

Technology, Chennai, India, 2019.

9\. R. Doriguzzi-Corin, S. Millar, S. Scott-Hayward, J. Martínez-del-Rincón and D. Siracusa, "Lucid: A Practical,

Lightweight Deep Learning Solution for DDoS Attack Detection," in IEEE Transactions on Network and Service

Management, vol. 17, no. 2, pp. 876-889, June 2020, doi: 10.1109/TNSM.2020.2971776.

10\. Madhavan, S. (2021, July 13). Introduction to convolutional neural networks. IBM developer. Retrieved January 5,

2023, from ttps://developer.ibm.com/articles/introduction-to-convolutional-neural-networks/

11\. Brownlee, J. (2020, August 20). A gentle introduction to the rectified linear unit (ReLU).

MachineLearningMastery.com. Retrieved December 18, 2022, from https://machinelearningmastery.com/rectified-

linear-activation-function-for-deep-learning-neural-networks/

o Data was used from the Canadian Institute of Cybersecurity’s (CIC)

DDoS Evaluation Dataset released in 2019

o CICDDoS2019 contains benign and the most up-to-date

common DDoS attacks, which resembles the true real-world

data (PCAPs).

o Ideal for deep learning models because of variety of attacks

and headers.

o Materials:

**5**

The final model resulted in ~~a 64-kernel convolutional model trained over 20000 flows of data~~.(Figure 6)

\- In the training phase, the model goes over a grid of hyperparameters, maximum 1000 epochs for each point in the grid. The

training process can stop earlier if no progress towards the minimum loss is observed for PATIENCE=10 consecutive epochs.

\- It achieved a training accuracy of **~~96.7%~~**

\- Performance (F1 score) is defined as the harmonic mean between precision and recall. It is used as a statistical measure to rate

performance: **~~96.4%~~**

o Computer

o Linux Mint VM

o Python Environment (using the Conda Framework and VSCode)

o Keras API easily builds layers in the CNN Model.

o Python wrapper for Pyshark, allowing python packet parsing

using Wireshark dissectors.

o Seaborn/Matplotlib functions to visualize data

o TensorFlow to build the model in Python

o Wireshark to visualize the packets in the dataset

o CIC Dataset (8)

12\. M. Roopak, G. Y. Tian and J. Chambers, "An Intrusion Detection System Against DDoS Attacks in IoT Networks,"

2020 10th Annual Computing and Communication Workshop and Conference (CCWC), Las Vegas, NV, USA, 2020,

pp. 0562-0567, doi: 10.1109/CCWC47524.2020.9031206.

13\. Sharma, S. (2022, November 20). Activation functions in neural networks. Medium. Retrieved January 22, 2023,

from https://towardsdatascience.com/activation-functions-neural-networks-1cbd9f8d91d6

**Fig. 6. Flow from the input (DDoS attack) to the various training layers, and output of ML algorithm predicting an attack**



<a name="br2"></a> 

**Supplementary Information**

Note: Figures are created from cited

sources or are my own

**Current Day State of the Art Drawbacks.**

**Code of CNN model**

**Code of Preprocessing Data**

Current detection approaches mostly use filtering (4) or rate limiting, which

can help in reducing some types of attacks such as spoofing IP addresses as

used by attackers to hide their identity but are not flexible when new attacks

are made and can slow down website performance speeds. Reactive

techniques are often required, and detection is needed to alert about the

attack to perform some automatic action. (Figure 6)

**Fig. 8: Flow Diagram of the current state of DDoS mitigation techniques**

Additionally, a problem in many solutions is that it is always challenging

to differentiate malicious flows from legitimate flows (5). In

commonplace networks, existing defense mechanisms against DDoS

attacks have limited success because they cannot meet the considerable

challenge of achieving simultaneously efficient detection, effective

response, acceptable rate of false alarm, and the real-time transfer of all

packets (6).

**Code of CNN model**

**Future Work**

1\.Implement the model in a real-world environment: The high accuracy of the model

suggests that it would be effective in a real-world setting, so implementing the model in a

network security system would be a crucial next step.

2\.Incorporate more data sources: Currently, the model is based on a single public dataset,

but incorporating data from additional sources, such as private datasets or real-time

network data, could further improve the model's accuracy and generalizability.

3\.Evaluate performance under different types of attacks: The current model has been

tested on a variety of attack types, but evaluating the model's performance on a larger and

more diverse set of attack types would provide a more comprehensive understanding of

its capabilities.

4\.Evaluate the impact of network characteristics on performance: The network

characteristics, such as network size and architecture, can impact the effectiveness of the

model. Evaluating the model's performance under different network conditions would

help understand the role that these factors play.

5\.Consider the impact of data preprocessing techniques: The data preprocessing

techniques used in this project, such as normalization and padding, are crucial to the

model's performance. Evaluating alternative preprocessing techniques and optimizing

these steps could lead to further improvements in the model's accuracy.

6\.Address interpretability and transparency concerns: As the model is used in security-

critical applications, understanding why the model makes certain predictions is important.

Research into methods for increasing the interpretability and transparency of the model's

predictions would be valuable.



<a name="br3"></a> 

Abstract

