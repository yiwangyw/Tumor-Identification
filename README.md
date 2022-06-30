<div id="top"></div>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->


<!-- PROJECT LOGO -->
<br />
<div align="center">

  <h3 align="center">Tumor Identification: Experimental Design for Machine Learning on Big Data</h3>
  <h4 align="center">By Yi Wang, Daniel Lin and Chen Wang</h4>

  <p align="center">
    Research to solve "How does one approach the problems with a big amount of data but without thousands of computing cores at one's disposal? What rigor has to be employed to make experiments robust in evaluations?"
    <br />
    <a href="https://github.com/yiwangyw/Tumor-Identification"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/yiwangyw/Tumor-Identification/issues">Report Bug</a>
    ·
    <a href="https://github.com/yiwangyw/Tumor-Identification/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

If the computing resource is limited, the data and network should be used fully. Referring to this [article](https://arxiv.org/pdf/1810.02328.pdf), we try to use Shannon’s communication model applied to labeling in machine learning. A dataset is converted into a parameterization (i.e., network weights) in the encoding step and the original label related to the sample points will be rebuilt in the decoding step. The upper limit of information that the decoder can capture is what we want to find. The memory capacity developed from information theory can be defined as the capacity that a decoder could reconstruct the original information with parameterization and the knowledge of the data. The unit of memory capacity (or Memory Equivalent Capacity [MEC])is the same as the unit of information to evaluate the capacity of a machine learner that could “memorize” information. The method to measure memory capacity is referred to in this article.

<br />

However, simply pursuing memorization will lead to overfitting. The generalization capacity, which is quantified by measuring accuracy against a validation set, should increase when the memory capacity of a network reduces. Data contains the information(signal) and noise. When the noises of data are cut down, the network with lower memory capacity (loss of data) and higher generalization can work better in a validation set. Likes the memory capacity, the unit of generalization capacity is ‘bit’ as well.

<br />

The experiment is designed to make a balance between memory and generalization in a specific task and try to use theory to explain them.  The noise in the data and Memory Equivalent Capacity (MEC) for the data has been studied. And we train the neural network for memorization to find limits of model memory and for generalization to find the best model MEC for accuracy. 

<br />

Additionally, we study the resilience of data. Resilience represents the capacity of that data to resist noise. The impact is as similar as generalization capacity.

<br />

The aim of this experiment is not only for accuracy but for developing rigor and interpretability in the neural network. 


<br />

When we try to train the network in memorization, the model could not reach memorization because we generate the feature map and removed some noise. It illustrates the effect of noise and information on machine learner training results, which needs to be further investigated. The memory capacity/generalization capacity can be rigor to evaluate a machine leaner.


<p align="right">(<a href="#top">back to top</a>)</p>



### Built With

This section should list any major frameworks/libraries used to bootstrap your project. Leave any add-ons/plugins for the acknowledgements section. Here are a few examples.

* [brainome](https://www.brainome.ai/)
* [Pytorch](https://pytorch.org/)

The dataset is from:

* [Kaggle: Skin Cancer: Malignant vs. Benign](https://www.kaggle.com/datasets/fanconic/skin-cancer-malignant-vs-benign)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

All source code is located in the "main". Run it as you would a normal jupyter notebook. 

### Prerequisites

* numpy
  ```sh
  pip install numpy
  ```
  
* scipy
  ```sh
  pip install scipy
  ```



<!-- USAGE EXAMPLES -->
## Usage

This project uses a pre-trained ResNet50 to determine if the tumor is benign or malignant to prove that MEC and other rigors are effective. If you would like to use the algorithms implemented please cite us.

<p align="right">(<a href="#top">back to top</a>)</p>






<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Project Link: [https://github.com/yiwangyw/Tumor-Identification](https://github.com/yiwangyw/Tumor-Identification)

<p align="right">(<a href="#top">back to top</a>)</p>





