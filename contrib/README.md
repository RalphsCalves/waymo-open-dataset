<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://waymo.com/blog/2020/03/announcing-waymos-open-dataset-challenges.html">
    <img src="images/logo.png" alt="Logo" width="320" height="180">
  </a>

<h3 align="center">Waymo Open Dataset Challenge Contribution</h3>

  <p align="center">
    Photo credits to Waymo Open Dataset. 
    README.md template credits to "Best-README-Template".
    <br />
    <a href="https://github.com/RalphsCalves/waymo-open-dataset"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/RalphsCalves/waymo-open-dataset">View Demo</a>
    ·
    <a href="https://github.com/RalphsCalves/waymo-open-dataset/issues">Report Bug</a>
    ·
    <a href="https://github.com/RalphsCalves/waymo-open-dataset/issues">Request Feature</a>
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

<!-- [![Product Name Screen Shot][product-screenshot]](https://example.com) -->

The purpose of this contribution folder is to add customized driver files, scripts, and test bench results from the work provided by the team. 

<p align="right">(<a href="#readme-top">back to top</a>)</p>


### Built With
> This project uses the following libraries and utilities. Each link to the installation page of each software

[![Google Colab][GoogleColab.js]][GoogleColab-url]
[![Python][Python.js]][Python-url]
[![Numpy][Numpy.js]][Numpy-url]
[![MatPlotLib][MatPlotLib.js]][MatPlotLib-url]
[![Pandas][Pandas.js]][Pandas-url]

[![TensorFlow][Tensorflow.js]][TensorFlow-url]
[![Tensorflow_graphics][Tensorflow_graphics.js]][Tensorflow_graphics-url]
[![Tensorflow_probability][Tensorflow_probability.js]][Tensorflow_probability-url]


[![OpenCV][OpenCV.js]][OpenCV-url]
[![SkiKitLearn][SkiKitLearn.js]][SkiKitLearn-url]
[![Plotly][Plotly.js]][Plotly-url]


<!-- [![Docker][Docker.js]][Docker-url] -->
<!-- [![Jira][Jira.js]][Jira-url] bruh... -->
<!-- [![OpenAI][OpenAI.js]][OpenAI-url] -->
<!-- [![Jupyter][Jupyter.js]][Jupyter-url] -->
<!-- [![PyTorch][Pytorch.js]][Pytorch-url] -->

<p align="right">(<a href="#readme-top">back to top</a>)</p>


### Folder Structure
> This folder structure includes this cloned repository and the relative location of the downloaded datasets provided by Waymo Open Dataset. The dataset must be downloaded seperately.

    . waymo-open-dataset
    ├── contrib             # Contributions to Waymo Open Dataset
    │   ├── scripts         # Python scripts (.py) for Command Line prompting
    │   ├── test_bench      # Python notebooks (.ipynb) for Google Collab test benches
    │   ├── utils           # Utilies, models, scripts, etc
    │   ├── README.md       # The file you are reading right now
    │   └── ...             # etc.
    ├── docs                # Waymo Documentation files and docs
    ├── src                 # Waymo Source files and libraries
    ├── tutorial            # Waymo Automated tests 
    ├── LICENSE
    └── README.md

    . perception-data       # Waymo perception data
    . motion-data           # Waymo motion data
<p align="right">(<a href="#readme-top">back to top</a>)</p>




<!-- GETTING STARTED -->
## Getting Started
Follow the steps below. 

### Download, Installation, Setup

1. Clone the repo
    ```sh
    git clone https://github.com/RalphsCalves/waymo-open-dataset.git
    ```

2. Install the required dependencies using 
    ```sh
    pip install -r requirements.txt
    ```
    or Setup Python Environment on Anaconda Navigator
    - Open Anaconda Navigator
    - Create new environment
    - Import packages from .yaml file
    - Open Environment in Jupyter

3. Download some waymo-open-dataset data 
    - [Motion Dataset v1.2: March 2023](https://console.cloud.google.com/storage/browser/waymo_open_dataset_motion_v_1_2_0)
    - [Perception Dataset v2.0.0: August 2023](https://console.cloud.google.com/storage/browser/waymo_open_dataset_v_2_0_0)

4. Preview Challenges and run Waymo tutorials to get an understanding of the functionality

    | Perception                     | 2D                                    | 3D                               |
    | --                             | --                                    | --                               |
    | Detection                      | [2D][Detection2D-url]                 | [3D][Detection3D-url]            |
    | Tracking                       | [2D][Tracking2D-url]                  | [3D][Tracking3D-url]             |
    | Real-Time Detection            | [2D][RTDetection2D-url]               | [3D][RTDetection3D-url]          |
    | Domain Adaptation              | ------                                | [3D][DomainAdaptation3D-url]     |
    | Camera Only 3D Detection       | ------                                | [3D][CameraOnlyDetection3D-url]  |
    | 2D Video Panoptic Segmentation | [2D][VideoPanopticSegmentation2D-url] | ------                           |
    | 3D Semantic Segmentation       | ------                                | [3D][SemanticSegmentation3D-url] |
    | KeyPoints                      | [2D][Keypoints2D-url]                 | ------                           |


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage
There are two methods of usage:
- Google Collab test bench
- Command Line prompting _(not yet available)_


### Steps
Each approach follows the same format of steps
1. Data Loading, Rasterizing, Preprocessing
2. Model Selection
3. Training
4. Inference, Validation, and Hyperparameter Tuning
5. Evaluation and Post-processing
6. Visualize and Submission

### Run Demo 
> If you are able to successfully run the demo, then functionality works as intended. Else, you may have the wrong set up. Make sure to have all pre-requisites installed correctly.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
<!-- ## Roadmap

- [] Feature 1
- [ ] Feature 2
- [ ] Feature 3
-   ested Feature

See the [open issues](https://github.com/RalphsCalves/waymo-open-dataset/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p> -->



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

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
<!-- ## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p> -->

<!-- CONTACT -->
<!-- ## Contact

Your Name - [@twitter_handle](https://twitter.com/twitter_handle) - email@email_client.com

Project Link: [https://github.com/RalphsCalves/waymo-open-dataset](https://github.com/RalphsCalves/waymo-open-dataset)

<p align="right">(<a href="#readme-top">back to top</a>)</p> -->

<!-- ACKNOWLEDGMENTS -->
<!-- ## Acknowledgments

* []()
* []()
* []()

<p align="right">(<a href="#readme-top">back to top</a>)</p> -->



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/RalphsCalves/waymo-open-dataset.svg?style=for-the-badge
[contributors-url]: https://github.com/RalphsCalves/waymo-open-dataset/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/RalphsCalves/waymo-open-dataset.svg?style=for-the-badge
[forks-url]: https://github.com/RalphsCalves/waymo-open-dataset/network/members
[stars-shield]: https://img.shields.io/github/stars/RalphsCalves/waymo-open-dataset.svg?style=for-the-badge
[stars-url]: https://github.com/RalphsCalves/waymo-open-dataset/stargazers
[issues-shield]: https://img.shields.io/github/issues/RalphsCalves/waymo-open-dataset.svg?style=for-the-badge
[issues-url]: https://github.com/RalphsCalves/waymo-open-dataset/issues
[license-shield]: https://img.shields.io/github/license/RalphsCalves/waymo-open-dataset.svg?style=for-the-badge
[license-url]: https://github.com/RalphsCalves/waymo-open-dataset/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/screenshot.png


<!-- For markdown links: https://shields.io/badges/static-badge -->
<!--    - badgeContent: numpy-0.20.0-%#013243 -->
<!--    - style: for-the-badge -->
<!--    - logo: numpy -->
<!--    - logoColor: #013243 -->

<!-- For icons and colors: https://simpleicons.org/?q=waymo -->
[GoogleColab.js]: https://img.shields.io/badge/GoogleColab--%23F9AB00?style=for-the-badge&logo=googlecolab
[Python.js]: https://img.shields.io/badge/Python--%233776AB?style=for-the-badge&logo=python
[Tensorflow.js]: https://img.shields.io/badge/tensorflow-2.11.0-%25%23FF6F00?style=for-the-badge&logo=tensorflow&logoColor=%23FF6F00&color=%23FF6F00
[Tensorflow_graphics.js]: https://img.shields.io/badge/tensorflow_graphics-2021.12.3-%25%23FF6F00?style=for-the-badge&logo=tensorflow&logoColor=%23FF6F00&color=%23FF6F00
[Tensorflow_probability.js]: https://img.shields.io/badge/tensorflow_probability-0.19.0-%25%23FF6F00?style=for-the-badge&logo=tensorflow&logoColor=%23FF6F00&color=%23FF6F00
[PyTorch.js]: https://img.shields.io/badge/pytorch-V1.2.3-%23EE4C2C?style=for-the-badge&logo=Pytorch
[Jupyter.js]: https://img.shields.io/badge/jupyter-V1.2.3-%23F37626?style=for-the-badge&logo=Jupyter
[Docker.js]: https://img.shields.io/badge/Docker-1.2.3-%232496ED?style=for-the-badge&logo=docker
[OpenCV.js]: https://img.shields.io/badge/opencv-0.0.0-%25%235C3EE8?style=for-the-badge&logo=opencv&logoColor=%235C3EE8&color=%235C3EE8
[OpenAI.js]: https://img.shields.io/badge/OpenAI-1.2.3-%23412991?style=for-the-badge&logo=openai
[Jira.js]: https://img.shields.io/badge/Jira%20Tickets-1.2.3-%230052CC?style=for-the-badge&logo=jira
[Numpy.js]: https://img.shields.io/badge/numpy-1.21.5-%25%23013243?style=for-the-badge&logo=numpy&logoColor=%23013243&color=%23013243
[Pandas.js]: https://img.shields.io/badge/pandas-1.5.3-%25%23150458?style=for-the-badge&logo=pandas&color=%23150458
[Plotly.js]: https://img.shields.io/badge/plotly-5.13.1-%25%233F4F75?style=for-the-badge&logo=plotly&color=%233F4F75
[SkiKitLearn.js]: https://img.shields.io/badge/scikitlearn-1.2.2-%25F7931E?style=for-the-badge&logo=scikitlearn&color=F7931E
[MatPlotLib.js]: https://img.shields.io/badge/matplotlib-3.6.1-%25%233776AB?style=for-the-badge&logo=python&logoColor=%233776AB&color=%233776AB


<!-- Link to the releases and installation pages of the following websites -->
[GoogleColab-url]: google.com
[Python-url]: python.org
[TensorFlow-url]: Tensorflow.org
[PyTorch-url]: pytorch.org
[Jupyter-url]: Jupyter.org
[Docker-url]: Docker.org
[OpenCV-url]: OpenCV.org
[OpenAI-url]: OpenAI.com
[Jira-url]: Jira.com
[Numpy-url]: Numpy.org
[Pandas-url]: Pandas.org
[Plotly-url]: Plotly.org
[SkiKitLearn-url]: SkiKitLearn.org
[MatPlotLib-url]: matplotlib.org
[Tensorflow_graphics-url]: tensorflow.com
[Tensorflow_probability-url]: tensorflow.com

<!-- Link to Waymo Challenges -->
[Detection2D-url]: https://waymo.com/intl/en_us/open/challenges/2020/2d-detection/
[Detection3D-url]: https://waymo.com/intl/en_us/open/challenges/2020/3d-detection/
[Tracking2D-url]: https://waymo.com/intl/en_us/open/challenges/2020/2d-tracking/
[Tracking3D-url]: https://waymo.com/intl/en_us/open/challenges/2020/3d-tracking/
[RTDetection2D-url]: https://waymo.com/intl/en_us/open/challenges/2021/real-time-2d-prediction/
[RTDetection3D-url]: https://waymo.com/intl/en_us/open/challenges/2021/real-time-3d-prediction/
[DomainAdaptation3D-url]: https://waymo.com/intl/en_us/open/challenges/2020/domain-adaptation/
[CameraOnlyDetection3D-url]: https://waymo.com/intl/en_us/open/challenges/2022/3d-camera-only-detection/
[VideoPanopticSegmentation2D-url]:https://waymo.com/intl/en_us/open/challenges/2023/2d-video-panoptic-segmentation/
[SemanticSegmentation3D-url]:https://waymo.com/intl/en_us/open/challenges/2022/3d-semantic-segmentation/
[Keypoints2D-url]:https://waymo.com/intl/en_us/open/challenges/2023/pose-estimation/