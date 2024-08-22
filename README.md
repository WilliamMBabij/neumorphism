# William Michael Babij's Portfolio

> Personal website and portfolio built with Jekyll and Neumorphism design.

## Table of Contents

- [About The Project](#about-the-project)
  - [Built With](#built-with)
  - [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
  - [Running Locally](#running-locally)
  - [Personalization and Customization](#personalization-and-customization)
    - [_config.yml](#_configyml)
    - [Github Metadata Plugin](#github-metadata-plugin)
    - [_data/*.yml](#_datayml)
    - [Particles.js](#particlesjs)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## About The Project

This is the personal website and portfolio of William Michael Babij, built with `Jekyll` and hosted on `GitHub Pages`. The design is based on the Neumorphism trend and developed with a mobile-first approach. This site showcases my resume, portfolio, and various projects.

### Built With

- [Jekyll](https://jekyllrb.com/)
- [Neumorphism Design](https://uxdesign.cc/neumorphism-in-user-interfaces-b47cef3bf3a6)
- [GitHub Pages](https://pages.github.com/)

### Features

- Mobile-First Responsive Design
- Animated preloader animation
- Landing Page with animated background using [particles.js](https://vincentgarreau.com/particles.js/), a Typing Carousel, and animated social icons
- Dark Neumorphism Design on main content
- [Animations On Scroll](https://michalsnik.github.io/aos/)
- Filterable *Skills* word cloud
- [GitHub's API](https://developer.github.com/v3/) automatically populating the *Open Source Projects* section
- Gulp dev workflow with [BrowserSync](https://browsersync.io/), [Autoprefixer](https://autoprefixer.github.io/), and `JS` & `SCSS` minifying
- [Google Analytics](https://analytics.google.com/)

## Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

- [NodeJS](https://nodejs.org/en/)

  ```sh
  brew install node
  ```

  If you need to switch between Node versions regularly, consider installing Node via [Node Version Manager](https://github.com/nvm-sh/nvm/blob/master/README.md#manual-install).

- [Jekyll](https://jekyllrb.com/)

  ```sh
  gem install bundler jekyll
  ```

  For more information, refer to [Jekyll Installation](https://jekyllrb.com/docs/installation/).

- [Yarn](https://yarnpkg.com/)

  ```sh
  npm install -g yarn
  ```

### Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/williammbabij/neumorphism.git
   ```

2. Change directory into the project folder:

   ```sh
   cd neumorphism
   ```

3. Install dependencies:

   ```sh
   yarn
   bundle install
   ```

## Usage

### Running Locally

Run and develop locally with a live server at `http://localhost:4000`. This will also build production-ready `JS` and `SCSS` assets with every change.

```sh
gulp
```

### Personalization and Customization

#### _config.yml

Edit `_config.yml` to personalize your site. For documentation, refer to [docs/config.md](https://github.com/longpdo/neumorphism/blob/master/docs/config.md).

#### Github Metadata Plugin

To automatically have your GitHub repositories pulled for the *Open Source Projects* section, authenticate yourself for the GitHub Metadata plugin.

1. Generate a new personal access token on GitHub:
   - Go to the [GitHub Token site](https://github.com/settings/tokens/new)
   - Select the scope `public_repository`, and add a description.
   - Confirm and save the settings. Copy the token you see on the page.

2. Create a `.env` file inside your repository and add your generated `JEKYLL_GITHUB_TOKEN`:

   ```text
   JEKYLL_GITHUB_TOKEN=0YOUR0GENERATED0TOKEN0
   ```

3. Change the value of `repository` inside `_config.yml` to your repository name.

#### _data/*.yml

Edit files inside `_data` to add information to the portfolio. For documentation, refer to [docs/data.md](https://github.com/longpdo/neumorphism/blob/master/docs/data.md).

#### Particles.js

Edit `assets/particles.json` to customize the landing page background animation. For more information, refer to [Particles.js Options](https://github.com/VincentGarreau/particles.js/#options).

## Deployment

To deploy the site, push your changes to the `main` branch on GitHub. GitHub Pages will automatically build and publish the site.

1. Commit your changes:

   ```sh
   git add .
   git commit -m "Your commit message"
   ```

2. Push to GitHub:

   ```sh
   git push origin main
   ```

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Acknowledgements

- [Jekyll](https://jekyllrb.com/)
- [Neumorphism Design](https://uxdesign.cc/neumorphism-in-user-interfaces-b47cef3bf3a6)
- [GitHub Pages](https://pages.github.com/)
- [Particles.js](https://vincentgarreau.com/particles.js/)
- [Animations On Scroll](https://michalsnik.github.io/aos/)
- [BrowserSync](https://browsersync.io/)
- [Autoprefixer](https://autoprefixer.github.io/)
- [Google Analytics](https://analytics.google.com/)