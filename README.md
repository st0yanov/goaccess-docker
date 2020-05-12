[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![License: GPLv3][license-shield]][license-url]

<br />
<p align="center">
  <h3 align="center">GoAccess Docker Compose</h3>

  <p align="center">
    Docker Compose skeleton project for GDPR compliant web analytics via <a href="https://goaccess.io/">GoAccess</a>.
    <br />
    <br />
    <a href="https://github.com/veskoy/goaccess-docker/issues">Report Bug</a>
    ·
    <a href="https://github.com/veskoy/goaccess-docker/issues">Request Feature</a>
  </p>
</p>

## Table of Contents

* [About the Project](#about-the-project)
  * [Built With](#built-with)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
* [Usage](#usage)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#contact)

## About The Project

This project aims to provide an example Docker Compose skeleton for setting up GDPR compliant web analytics via a tracking pixel.

### Built With
* [Docker](https://www.docker.com/)
* [Docker Compose](https://docs.docker.com/compose/)

## Getting Started

To get a local copy up and running follow these simple example steps.

### Prerequisites

* Docker
* Docker Compose

### Installation

1. Clone the repo
```sh
git clone https://github.com/veskoy/goaccess-docker.git
```
2. Create a website configuration file
```sh
mv nginx/sites-available/example.com.conf nginx/sites-available/yoursite.com.conf
```
3. Alter the `server_name`, `access_log` and `root` values appropriately
4. Adjust the `goaccess/html` volume and goaccess command `--log-file=` inside `docker-compose.yml`

## Usage

Run the project:
```sh
docker-compose up
```

Tracking pixel is accessible on http://yoursite.com/stats.gif while the analytics web interface could be found on http://yoursite.com/index.html (you can serve it wherever you want).

## Roadmap

See the [open issues](https://github.com/veskoy/goaccess-docker/issues) for a list of proposed features (and known issues).

## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

License: GPL v3
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

## Contact

Veselin Stoyanov:
[![LinkedIn][linkedin-shield]][linkedin-url]

[contributors-shield]: https://img.shields.io/github/contributors/veskoy/goaccess-docker.svg?style=flat-square
[contributors-url]: https://github.com/veskoy/goaccess-docker/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/veskoy/goaccess-docker.svg?style=flat-square
[forks-url]: https://github.com/veskoy/goaccess-docker/network/members
[stars-shield]: https://img.shields.io/github/stars/veskoy/goaccess-docker.svg?style=flat-square
[stars-url]: https://github.com/veskoy/goaccess-docker/stargazers
[issues-shield]: https://img.shields.io/github/issues/veskoy/goaccess-docker.svg?style=flat-square
[issues-url]: https://github.com/veskoy/goaccess-docker/issues
[license-shield]: https://img.shields.io/badge/License-GPLv3-blue.svg
[license-url]: https://www.gnu.org/licenses/gpl-3.0
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?logo=linkedin&color=blue
[linkedin-url]: https://www.linkedin.com/in/stoyanovv/
