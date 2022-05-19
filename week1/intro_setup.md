# 📋 Week 1 Notes: Intro & Environment Setup

When you are designing a machine learning system, your job doesn't end with building the model—and achieving a high accuracy score and a low validation error! For the model to be actually helpful—you will have to consider deploying it, and also ensure that the model's performance does not degrade over time. And MLOps is a set of *best practices* for putting machine learning models into production.

![image](https://user-images.githubusercontent.com/47279635/168582280-52820583-d0bb-4b46-add4-b2fa4c09bc1b.png)

## 🎯 Steps in a Machine Learning Project
The various stages in a machine learning project can be broadly captured in the following three steps:
1. **Design**: In the `design` step, you are considering the problem at hand—to decide whether or not you'll need a machine learning algorithm to achieve the objective. 
2. **Train**: Once you decide on using a machine learning algorithm, you `train` the model and optimize its performance on the validation dataset.
3. **Operate**: The `operate` state captures the performance of the model after it's deployed. Some of the questions that you'll answer throughout the course, include:
  - If the performance of the model degrades, can you retrain the model in a cost-effective manner?
  - How do you ensure that the deployed model performs as expected—that is, how do you monitor the model's performance in production?
  - What are the challenges associated with monitoring ML models?

## ⚙ Environment Setup

Recommended development environment: Linux

### 1. Download and install the Anaconda distribution of Python
```sh
$ wget https://repo.anaconda.com/archive/Anaconda3-2022.05-Linux-x86_64.sh

```

### 2. Update existing packages
```sh
$ sudo apt update
```
### 3. Install Docker
```sh
$ sudo apt install docker.io
```

### 4. Install Docker Compose

4.1 Install docker-compose in a separate directory
```sh
$ mkdir soft
$ cd soft
```

4.2 To get the latest release of Docker Compose, go to https://github.com/docker/compose and download the release for your OS.

```sh
$ wget https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64 -O docker-compose
```
4.3 Make it executable
```sh
$ chmod +x docker-compose
```
4.4 Add to path
```sh
$ nano .bashrc
# In .bashrc, add:
export PATH="${HOME}/soft:${PATH}"
# Run
$ source .bashrc
```

### [Optional] Run Docker without `sudo`
```sh
$ sudo groupadd docker
$ sudo usermod -aG docker $USER
```
### 5. Run Docker
```sh
$ docker run hello-world
```
