# CMSC828I-Advanced-Techniques-in-Visual-Learning-Recognition
This repository serves as a record of my academic experience in CMSC828 during the Fall of 2023. It includes my code submissions for assignments and projects. Each assignment is organized within its respective folder, complete with accompanying documentation and any necessary resources.

## 📚 Course Overview
The course offers a deep dive into the cutting-edge realms of computer vision and high-level recognition tasks. This course is structured into five key modules, each addressing a crucial aspect of visual learning and recognition:

1. **Background and Foundations:** Introduction to Data, covering topics like the massive 80 million tiny image dataset and the storage capacity of visual long-term memory. Data-driven methods in vision, including image restoration, scene completion, and geographic information estimation from images. Exploring ConvNets and architectures, with a focus on various important architectures and the inner workings of convolutional neural networks.

2. **Core Tasks:** Foundational topics in Object Detection and Image Segmentation, including Histograms of Oriented Gradients and object detection with part-based models. Single-stage object detection techniques like OverFeat, SSD, and YOLO, as well as semantic segmentation methods. Multi-stage object detection and instance segmentation using approaches like Fast R-CNN, Faster R-CNN, and Mask R-CNN. Introduction to transformers for detection/segmentation. Analysis, diagnosis, and training strategies for object detectors.

4. **Additional Topics:** Introduction to other tasks like Human Pose Estimation. Guest lecture on Reinforcement Learning. Self-supervised Learning. Learned Compression techniques beyond images and video. Neural Architecture Search for efficient model design. Vision Techniques for Reinforcement Learning. Action Recognition methods. Attribute recognition. Context reasoning in object recognition.

5. **Guest Lectures:** Guest lectures covering topics like self-supervised learning, learned compression, neural architecture search, vision techniques for reinforcement learning, action recognition, attributes, and context reasoning.

6. **Generative Models and More:** In-depth exploration of 3D Scene Understanding, Primitives, and Reasoning. Study of 3D object recognition, including 3D Scene Understanding, 3D object primitives, and reasoning. Generative Models for image and data generation. Miscellaneous topics related to visual data mining and discovery. Ethical considerations in computer vision.

Throughout the course, students will engage with a wide range of research papers, lectures, and assignments, providing them with a comprehensive understanding of advanced techniques in visual learning and recognition. The course covers foundational concepts, cutting-edge methods, and emerging trends in the field of computer vision and visual recognition.


## 📄 Assignment List
### [Assignment 1](https://github.com/Rishikesh-Jadhav/CMSC828I-Advanced-Techniques-in-Visual-Learning-Recognition/tree/main/Assignment1): Superpixels and Image Segmentation

### [Results](https://github.com/Rishikesh-Jadhav/CMSC828I-Advanced-Techniques-in-Visual-Learning-Recognition/blob/main/Assignment1/rjadhav1(119256534)cmsc828I_fall2023_HW1.ipynb) : Contains the notebook wih the outputs of the given task.

- **Learnings from Assignment 1**:
  
  1. **Dataset**:Used the Microsoft Research Cambridge Object Recognition Image Database (MSRC Object Categorization Dataset) for the assignment.
     
  2. **Superpixel Segmentation**: Understood the concept of superpixel segmentation, which involves grouping similar pixels into coherent regions or superpixels, simplifying image analysis.

  3. **SLIC Algorithm**: I learned about the SLIC (Simple Linear Iterative Clustering) algorithm, a popular method for superpixel generation, which was implemented from scratch.

  4. **Data Preparation**: Prepared data for the supepixel segmentation task, including organizing image and ground truth segmentation files and splitting the data into training and testing sets.

  5. **Patch Extraction**: Learned how to extract superpixel patches along with their class labels. This process involved bounding box extraction, label assignment based on the majority class, and saving patches in a suitable format.

  6. **Data Loading**: Created a custom dataset class for loading superpixel patches and their labels, making the data ready for training deep learning models.

  7. **Deep Learning**: Used PyTorch to define a deep learning model for superpixel classification, and I learned to fine-tune a pre-trained model (ResNet) for this specific task.

  8. **Training and Evaluation**: Trained and evaluated the model, including tracking training and testing losses and accuracies over multiple epochs.

  9. **Data Visualization**: Visualized images, superpixel patches, and segmentation maps.

  10. **Optimization and Learning Rate Scheduling**: I set up an optimizer (Adam) and a learning rate scheduler to fine-tune the model's performance.

  11. **Random Splitting**: The assignment involved splitting the dataset into training and testing subsets to assess the model's performance.

  12. **Bonus Learning**: I explored the possibility of improving the model by implementing more advanced techniques like feature fusion or multi-resolution networks.

  13. **Flexibility**: The assignment allowed me to demonstrate flexibility in implementing different aspects of the project, such as adapting code for custom datasets and tasks, handling small patches, and ensuring efficient data   processing.


## Additional Resources
- [Course related resources](https://www.cs.umd.edu/class/fall2023/cmsc828i/)


