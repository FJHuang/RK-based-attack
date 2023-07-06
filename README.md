# Adversarial Attack Based on Runge-Kutta Method
This repository contains the code for Adversarial Attack Based on Runge-Kutta Method.

Deep neural networks (DNNs) have made remarkable achievements in many fields, but related studies show that they are vulnerable to adversarial examples. The gradient-based attack is a popular adversarial attack and has attracted wide attention. This study investigates the relationship between gradient-based adversarial attacks and numerical methods for solving ordinary differential equations (ODEs). In addition, it proposes a new adversarial attack based on Runge-Kutta (RK) method, a numerical method for solving ODEs. According to the prediction idea in the RK method, perturbations are added to the original examples first to construct predicted examples, and then the gradients of the loss functions with respect to the original and predicted examples are linearly combined to determine the perturbations to be added for the generation of adversarial examples. Different from the existing adversarial attacks, the proposed adversarial attack employs the prediction idea of the RK method to obtain the future gradient information (i.e., the gradient of the loss function with respect to the predicted examples) and uses it to determine the adversarial perturbations to be added. The proposed attack features good extensibility and can be easily applied to all available gradient-based attacks. Extensive experiments demonstrate that in contrast to the state-of-the-art gradient-based attacks, the proposed RK-based attack boasts higher success rates and better transferability.

Requirements

- Python 3.6.5
- Tensorflow 1.12.0 
- Numpy 1.15.4 
- Opencv2 3.4.2

Running the code

 python rk3_fgsm.py:  generate adversarial examples for Inception_V3 using RK3-FGSM.
 python rk4_fgsm.py:  generate adversarial examples for Inception_V3 using RK4-FGSM. 

Models

Inception_V3 
http://download.tensorflow.org/models/inception_v3_2016_08_28.tar.gz

Inception_V4 
http://download.tensorflow.org/models/inception_v4_2016_09_09.tar.gz

Inception_ResNet_V2 
http://download.tensorflow.org/models/inception_resnet_v2_2016_08_30.tar.gz

ResNet_V2_152 
http://download.tensorflow.org/models/resnet_v2_152_2017_04_14.tar.gz




Example usage

- Generate adversarial examples:
 python rk3_fgsm.py
 python rk4_fgsm.py


中文引用格式: 万晨, 黄方军. 基于龙格库塔法的对抗攻击方法. 软件学报. http://www.jos.org.cn/1000-9825/6893.htm

英文引用格式: Wan C, Huang FJ. Adversarial Attack Based on Runge-Kutta Method. Ruan Jian Xue Bao/Journal of Software (in Chinese). http://www.jos.org.cn/1000-9825/6893.htm
