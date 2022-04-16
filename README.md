[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<br />
<div align="center">
  <a href="https://github.com/celikfatih/jupyter-docker-compose/">
    <img src="images/main-logo.svg" alt="Logo" width="80" height="80">
  </a>

<h3 align="center">Jupyter Docker Compose</h3>

  <p align="center">
    It is a Jupyter Notebook environment built using docker-compose.
    <br />
    <a href="https://github.com/celikfatih/jupyter-docker-compose/">
    <br />
    <a href="https://github.com/celikfatih/jupyter-docker-compose/issues">Report Bug</a>
    ·
    <a href="https://github.com/celikfatih/jupyter-docker-compose/issues">Request Feature</a>
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
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

## About The Project

In this project, `jupyter/scipy-notebook` is used as docker image. scipy-notebook includes popular packages from the scientific Python ecosystem scipy-notebook contains the following packages:

- altair
- beautifulsoup4
- bokeh
- bottleneck
- cloudpickle
- conda-forge::blas=\*=openblas
- cython
- dask
- dill
- h5py
- matplotlib-base
- numba
- numexpr
- pandas
- patsy
- protobuf
- pytables
- scikit-image
- scikit-learn
- scipy
- seaborn
- sqlalchemy
- statsmodel
- sympy
- widgetsnbextension
- xlrd
- ipympl
- ipywidgets
- Facets for visualizing machine learning datasets

It was created as docker-compose to use external docker images with scipy-notebook.

## Getting Started

To run locally, follow the steps below.

### Prerequisites

To run locally, you must first have `docker` and `docker-compose`.

- [Here's](https://docs.docker.com/desktop/) how to download Docker to your local environment.
- [Here's](https://docs.docker.com/compose/install/) how to download Docker Compose to your local environment.

### Installation

1. First of all, it should be checked that `docker` and `docker-compose` are running.

2. Clone the repo:
   ```sh
   git clone https://github.com/celikfatih/jupyter-docker-compose.git
   ```
3. Specify the values of the parameters in the `.env` file.

   - `WORKING_DIR`: The path where the created project files will be saved (ex: `Users/root/jupyter-workspace`).
   - `DATASET_DIR`: The path to the datasets to work with. (ex: `Users/root/jupyter-workspace/datasets`)
   - `PASSWORD`: Password to access jupyter-notebook.
   - `PORT`: Port to use to access jupyter-notebook.

4. Inside the project, to start jupyter (The `-d` parameter optional and allows it to run in the background):
   ```sh
   docker-compose up -d
   ```
5. If you don't get any error, go to `http://localhost:{PORT}` or `http://127.0.0.1/{PORT}`.

## Usage

If you were able to access the Jupyter Notebook UI when you went to the address, enter your password on the screen.

When you access Jupyter Notebook, check if the `WORKING_DIR` and `DATASET_DIR` you have specified appear on the screen. If a problem does not appear, you can start your work.

By accessing your data from the location you specified, you can do all your work, and your work will also be saved in the location you specified.

## Roadmap

- [x] Add Scipy-Notebook
- [ ] Add Additional Notebook Types
- [ ] Add different components will be added to work with Jupyter.
  - [ ] Spark
  - [ ] Flink
  - [ ] Celery etc.

See the [open issues](https://github.com/celikfatih/jupyter-docker-compose/issues) for a full list of proposed features (and known issues).

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the GNU General Public License v3.0. See `LICENSE` for more information.

## Contact

Fatih Celik - [@celikfatii](https://twitter.com/celikfatii) - celikfatih@protonmail.com

Project Link: [https://github.com/celikfatih/jupyter-docker-compose/](https://github.com/celikfatih/jupyter-docker-compose/)

## Acknowledgments

- [Img Shields](https://shields.io)
- [Best-README-Template](https://github.com/othneildrew/Best-README-Template)

[contributors-shield]: https://img.shields.io/github/contributors/celikfatih/jupyter-docker-compose.svg?style=for-the-badge
[contributors-url]: https://github.com/celikfatih/jupyter-docker-compose/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/celikfatih/jupyter-docker-compose.svg?style=for-the-badge
[forks-url]: https://github.com/celikfatih/jupyter-docker-compose/network/members
[stars-shield]: https://img.shields.io/github/stars/celikfatih/jupyter-docker-compose.svg?style=for-the-badge
[stars-url]: https://github.com/celikfatih/jupyter-docker-compose/stargazers
[issues-shield]: https://img.shields.io/github/issues/celikfatih/jupyter-docker-compose.svg?style=for-the-badge
[issues-url]: https://github.com/celikfatih/jupyter-docker-compose/issues
[license-shield]: https://img.shields.io/github/license/celikfatih/jupyter-docker-compose.svg?style=for-the-badge
[license-url]: https://github.com/celikfatih/jupyter-docker-compose/blob/master/LICENSE
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/cefatihcelik
