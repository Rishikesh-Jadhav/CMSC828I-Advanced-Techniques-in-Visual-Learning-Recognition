# CMSC828I-Advanced-Techniques-in-Visual-Learning-Recognition
This repository serves as a record of my academic experience in CMSC828 during the Fall of 2023. It includes my code submissions for projects. Each Project is organized within its respective folder, complete with accompanying documentation and any necessary resources.

## 📚 Course Overview
The course offers a deep dive into the cutting-edge realms of computer vision and high-level recognition tasks. This course is structured into five key modules, each addressing a crucial aspect of visual learning and recognition:

1. **Background and Foundations:** Introduction to Data, covering topics like the massive 80 million tiny image dataset and the storage capacity of visual long-term memory. Data-driven methods in vision, including image restoration, scene completion, and geographic information estimation from images. Exploring ConvNets and architectures, with a focus on various important architectures and the inner workings of convolutional neural networks.

2. **Core Tasks:** Foundational topics in Object Detection and Image Segmentation, including Histograms of Oriented Gradients and object detection with part-based models. Single-stage object detection techniques like OverFeat, SSD, and YOLO, as well as semantic segmentation methods. Multi-stage object detection and instance segmentation using approaches like Fast R-CNN, Faster R-CNN, and Mask R-CNN. Introduction to transformers for detection/segmentation. Analysis, diagnosis, and training strategies for object detectors.

4. **Additional Topics:** Introduction to other tasks like Human Pose Estimation. Guest lecture on Reinforcement Learning. Self-supervised Learning. Learned Compression techniques beyond images and video. Neural Architecture Search for efficient model design. Vision Techniques for Reinforcement Learning. Action Recognition methods. Attribute recognition. Context reasoning in object recognition.

5. **Guest Lectures:** Guest lectures covering topics like self-supervised learning, learned compression, neural architecture search, vision techniques for reinforcement learning, action recognition, attributes, and context reasoning.

6. **Generative Models and More:** In-depth exploration of 3D Scene Understanding, Primitives, and Reasoning. Study of 3D object recognition, including 3D Scene Understanding, 3D object primitives, and reasoning. Generative Models for image and data generation. Miscellaneous topics related to visual data mining and discovery. Ethical considerations in computer vision.

Throughout the course, we engaged with a wide range of research papers, lectures, and Projects, which providing us with a comprehensive understanding of advanced techniques in visual learning and recognition. The course covers foundational concepts, cutting-edge methods, and emerging trends in the field of computer vision and visual recognition.


## 📄 Project List

### [Project 1](https://github.com/Rishikesh-Jadhav/CMSC828I-Advanced-Techniques-in-Visual-Learning-Recognition/tree/main/Project1): Superpixels and Image Segmentation

### [Results](https://github.com/Rishikesh-Jadhav/CMSC828I-Advanced-Techniques-in-Visual-Learning-Recognition/blob/main/Project1/rjadhav1(119256534)cmsc828I_fall2023_HW1.ipynb) : Contains the notebook wih the outputs of the given task.

- **Implementation and Learnings from Project 1**:
  
  1. **Dataset**:Used the Microsoft Research Cambridge Object Recognition Image Database (MSRC Object Categorization Dataset) for the Project.
     
  2. **Superpixel Segmentation**: Understood the concept of superpixel segmentation, which involves grouping similar pixels into coherent regions or superpixels, simplifying image analysis.
     - #### Kmeans Clustering Output
     <img src="images/naive%20clustering.png" alt="Kmeans Clustering" width="20%"/>
  3. **SLIC Algorithm**: I learned about the SLIC (Simple Linear Iterative Clustering) algorithm, a popular method for superpixel generation, which was implemented from scratch.
     - #### SLIC Clustering with Enforced Constraints
     <img src="images/slic%20clustering.png" alt="SLIC Clustering" width="20%"/>
  4. **Data Preparation**: Prepared data for the supepixel segmentation task, including organizing image and ground truth segmentation files and splitting the data into training and testing sets.
     - #### Sample Patch of the Newly Created Dataset
     <img src="images/sample%20%20seg%20patch.png" alt="Sample Patch" width="20%"/>  
  5. **Patch Extraction**: Learned how to extract superpixel patches along with their class labels. This process involved bounding box extraction, label Project based on the majority class, and saving patches in a suitable format.

  6. **Data Loading**: Created a custom dataset class for loading superpixel patches and their labels, making the data ready for training deep learning models.

  7. **Deep Learning**: Used PyTorch to define a deep learning model for superpixel classification, and I learned to fine-tune a pre-trained model (ResNet) for this specific task.

  8. **Training and Evaluation**: Trained and evaluated the model, including tracking training and testing losses and accuracies over multiple epochs.

  9. **Data Visualization**: Visualized images, superpixel patches, and segmentation maps.
     - #### Output of ResNet-based Segmentation Model  
     <img src="images/seg%20rgb%20image.png" alt="RGB Image" width="45%"/>
     <img src="images/resnet%20prediction.png" alt="Segmentation Model Output + GT" width="20%"/>
    
  10. **Optimization and Learning Rate Scheduling**: I set up an optimizer (Adam) and a learning rate scheduler to fine-tune the model's performance.

  11. **Random Splitting**: The Project involved splitting the dataset into training and testing subsets to assess the model's performance.

  12. **Bonus Learning**: I explored the possibility of improving the model by implementing more advanced techniques like feature fusion or multi-resolution networks.

  13. **Flexibility**: The Project allowed me to demonstrate flexibility in implementing different aspects of the project, such as adapting code for custom datasets and tasks, handling small patches, and ensuring efficient data   processing.


### [Project 2](https://github.com/Rishikesh-Jadhav/CMSC828I-Advanced-Techniques-in-Visual-Learning-Recognition/tree/main/Project2): Implicit Neural Representation

### [Results](https://github.com/Rishikesh-Jadhav/CMSC828I-Advanced-Techniques-in-Visual-Learning-Recognition/blob/main/Project2/Rishikesh_cmsc828I_fall_2023_HW2.ipynb) : Contains the notebook wih the outputs of the given task.

- **Implementation and Learnings from Project 2**:
  
  1. **Understanding Implicit Neural Representation (INR)**: Explored hands-on experience with INR, parameterizing signals (images) with a neural network (feed-forward network in this Project).
  
  2. **SingleImageDataset Implementation**: Developed a `SingleImageDataset` to convert the selected image into model inputs and targets.
     - **Selected Image**  
     ![Selected Image](images/redbull%20rgb.png)

  3. **Image Resizing**: Resized the selected image to meet the maximum pixel count requirement, ensuring efficient model training.
  
  4. **Loop and DataLoader Implementation**: Implemented a loop to construct the image using a DataLoader for the `SingleImageDataset`.
  
  5. **Feedforward Neural Network Definition**: Defined a basic feedforward neural network (`FFN`) with appropriate layers and weights for INR.

  6. **Training Setup**: Configured the model training with an optimizer, criterion (pixel-wise MSE loss), and tracked loss over epochs.
  
  7. **Model Training**: Trained the network on the dataset until convergence, monitored loss, and adjusted learning rate using a scheduler.

  8. **Loss Plotting**: Plotted the loss values over epochs for visual analysis.
     - **Reconstruction Loss Vs Training Time**  
     ![Loss Plot](images/loss%20plot.png)
      
  10. **Image Reconstruction**: Reconstructed the image using the trained model’s outputs at each coordinate.
     - **Reconstructed Image with GT**  
     ![Reconstructed Image](images/image%20reconstruction.png)
      
  11. **Compute PSNR**: Computed PSNR for the reconstruction vs. the original image from scratch: PSNR: 65.75267791748047 dB
  
  12. **Outpainting**: Predicted 20 pixels in all directions outside the boundaries of the original image using the trained model.
     - **Outpainted Image with GT**  
     ![Outpainted Image](images/outpainting.png)
     
## Additional Resources
- [Course related resources](https://www.cs.umd.edu/class/fall2023/cmsc828i/)


