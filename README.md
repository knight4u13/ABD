<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a id="readme-top"></a>
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
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/knight4u13/ABD">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Adversarial Backdoor Defense in CLIP</h3>

  <p align="center">
    This repository contains the introduction of ABD and the development of CLIP Backdoor Security Platform:
    <br />
    <a href="https://github.com/knight4u13/ABD"><strong>Read Paper »</strong></a>
    <br />
    <br />
    <a href="https://github.com/knight4u13/ABD">View Platform</a>
    ·
    <a href="https://github.com/knight4u13/ABD/issues/new?assignees=&labels=bug&projects=&template=bug-report---.md">Report Bug</a>
    ·
    <a href="https://github.com/knight4u13/ABD/issues/new?assignees=&labels=enhancement&projects=&template=feature-request---.md">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#paper">Paper</a>
      <ul>
        <li><a href="#intro">Introduction</a></li>
        <li><a href="#method">Method</a></li>
        <li><a href="#evaluation">Evaluation</a></li>
      </ul>
    </li>
    <li>
      <a href="#platform">AI Security Platform</a>
      <ul>
        <li><a href="#ui">UI</a></li>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#quick start">Quick Start</a>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
# 📘 **ABD: Adversarial Backdoor Defense**
## Introduction
[Thesis Title：Adversarial Backdoor Defense in CLIP](https://arxiv.org/abs/2409.15968)  
This repository contains the code and implementation details for our paper **Adversarial Backdoor Defense in CLIP**.

> **Thesis Link**：[Link](https://arxiv.org/abs/2409.15968)  
> **Abstract**：
Multimodal contrastive pretraining, exemplified by models like CLIP, has been found to be vulnerable to backdoor attacks. While current backdoor defense methods primarily employ conventional data augmentation to create augmented samples aimed at feature alignment, these methods fail to capture the distinct features of backdoor samples, resulting in suboptimal defense performance. Observations reveal that adversarial examples and backdoor samples exhibit similarities in the feature space within the compromised models. Building on this insight, we propose Adversarial Backdoor Defense (ABD), a novel data augmentation strategy that aligns features with meticulously crafted adversarial examples. This approach effectively disrupts the backdoor association. Our experiments demonstrate that ABD provides robust defense against both traditional uni-modal and multimodal backdoor attacks targeting CLIP. Compared to the current state-of-the-art defense method, CleanCLIP, ABD reduces the attack success rate by 8.66% for BadNet, 10.52% for Blended, and 53.64% for BadCLIP, while maintaining a minimal average decrease of just 1.73% in clean accuracy.

[![Method Overview][Paper-image-1]](https://arxiv.org/abs/2409.15968)   
<!-- checkpoint: finish page -->
## **Core Methods**:
1. **Adversarial Example Generation**：Combine adversarial training with backdoor loss to generate samples that meet the backdoor triggering characteristics.  
2. **Data Augmentation**：Replace backdoor samples with adversarial samples to enhance the robustness of the model.  
3. **Efficient Defense**：Experiments show that ABD performs well in both traditional and CLIP-specific backdoor attacks, outperforming existing defense methods such as CleanCLIP. 
[![Iluustration][Paper-image-2]](https://arxiv.org/abs/2409.15968)  

## 📊 Experimental Results
<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

# ⚙️ Platform: ABD Defense Toolkit

> The platform provides a visual experiment and operation interface for the ABD method, supporting users to quickly test and reproduce the experimental results in the paper.

## **Main functions**  
- **Experimental visualization**：Show the comparison between adversarial samples and backdoor samples, the changing trend of model performance, etc. 
- **Model fine-tuning and evaluation**：Provides one-click model fine-tuning and testing functions, supporting CLIP models. 
- **Data processing and analysis**：Contains functional modules such as backdoor sample insertion, adversarial perturbation generation, and result statistics.

## **UI**  
**Main UI**
[![Main ui][Main-ui]](https://arxiv.org/abs/2409.15968)   

**Submit UI**
[![Sub ui][Sub-ui]](https://arxiv.org/abs/2409.15968)    


## **Built With**  
* [![Pytorch][Pytorch.com]][Pytorch-url]
* [![Flask][Flask.com]][Flask-url]
* [![LayUI][LayUI.com]][LayUI-url]
* [<img src="https://res.layui.dev/static/images/layui/logo.png" alt="LayUI" height="28">][LayUI-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

# 🚀 Quick Start  

1. **Clone Projects**  
```bash  
git clone https://github.com/knight4u13/ABD.git  
cd ABD-CLIP-Platform 
```

2. **Install Dependencies** 
```bash
pip install -r requirements.txt
```

3. **Run the Platform** 
```bash
pip main.py
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

# 🤝 Contributing

We welcome contributions to improve the platform or extend its capabilities. Please open an issue or submit a pull request!

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

# License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

# 📧 Contact

For questions, feel free to contact us at `kuangjh6@mail2.sysu.edu.cn`.

Project Link: [https://github.com/knight4u13/ABD](https://github.com/knight4u13/ABD)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---

# Acknowledgments

Some portions of the code in this repository are adaptations from the following repositories:

* [CleanCLIP](https://github.com/nishadsinghi/CleanCLIP)
* [mlfoundations](https://github.com/mlfoundations/open_clip)
* [openai](https://github.com/openai/CLIP)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

---
<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 

<!-- added by kjh -->
[Paper-image-1]: images/advdefense.png
[Paper-image-2]: images/advexplanation.png
[Main-ui]: images/visualization.png
[Sub-ui]: images/defense.png
[Flask.com]: https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=Flask&logoColor=white
[Flask-url]: https://flask.palletsprojects.com/en/stable/
[Pytorch.com]: https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white
[Pytorch-url]: https://flask.palletsprojects.com/en/stable/
[LayUI.com]: https://res.layui.dev/static/images/layui/logo.png
[LayUI-url]: https://flask.palletsprojects.com/en/stable/