# A Novel Deep Learning Solution to detect DDoS attacks using Neural Networks
Science Fair Project made by Vedanth Ramanathan, working with Professor Krish Mahadevan and Ms. Sejal Dua. Won US Army and Navy Excellence Awards. 3rd in Fair. Made using Python, LinuxMint, and Tensorflow. Achieved a Accuracy of 99.6% over 2000+ samples.
Link to Paper: https://arxiv.org/abs/2309.05646
Confusion Matrix:

![Confusion Matrix](Figure6.png?raw=true)

Thanks to the University of North Brunswick for providing a [state of the art dataset](https://www.unb.ca/cic/datasets/ddos-2019.html), to which I trained my model to.

Abstract: Cybersecurity attacks are becoming increasingly sophisticated and pose a growing threat to individuals, and private and public sectors. DDoS attacks are one of the most harmful of these threats in today’s Internet, disrupting the availability of essential services. This project presents a novel deep learning-based approach for detecting DDoS attacks in network traffic using the industry-recognized CICDDoS2019 dataset, which contains packet captures from real-time DDoS attacks, creating a broader and more applicable model for the real world. The algorithm employed in this study exploits the properties of Convolutional Neural Networks (CNN) and common deep learning algorithms to build a novel mitigation technique that classifies benign and malicious traffic. The proposed model preprocesses the data by extracting packet flows and normalizing them to a fixed length. The data is then fed into a CNN architecture consisting of a 2D convolutional layer with 64 filters, kernel size of 3x3, and kernel regularization, followed by layers regulating node dropout, normalization, and a sigmoid activation function to out a binary classification. This will allow for the model to process the pcaps effectively and look for the nodes that contribute to DDoS attacks while dropping the “noise” or the distractors. The results of this study demonstrate the effectiveness of the proposed algorithm in detecting DDOS attacks in network traffic as well as being scalable for any network environment. 

Project:

![Project pdf](ScienceFair2023Presentation.pdf?raw=true)


