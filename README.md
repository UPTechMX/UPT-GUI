# UPT-GUI

## Table of contents
- [Description](#description)
- [How To Use](#how-to-use)
- [References](#references)
- [License](#license)
- [Author Info](#author-info)


## Description

This project contains the Graphical User Interface or frontend of the Suitability and Urban Performance tools.

The Urban Planning Tool Suitability identifies optimal locations within a city for a specific activity by evaluating proximity between urban facilities and inhabitants, at local/ neighborhood levels across the city. It includes two search functionalities, the layer, and the filter, which correspond to indicators, planning standards, and national government’s norms essential for spatial planning (population, employment, density, land use, etc.). These functionalities allow flexibility to decision-makers, to explore multiple combinations of urban spatial planning parameters that capture and respond to the city’s needs and challenges.

The Urban Planning Tool Urban Performance assesses the city's present and future performance by modeling investment projects or policies in a range of indicators related to the Sustainable Development Goals (SDG), including aspects such as poverty reduction, water management, energy, infrastructure, public transportation, climate action, etc. Urban Performance models multiple scenarios and spatial solutions to test the effectiveness of their contributions to sustainable development. Scenarios can serve 


## Main Technologies Used:
- Angular

### Main Libraries Used:
- PrimeNG
- PrimeIcons
- Angular MDBootstrap
- Angular Material
- Font Awesome

## How To Use

### Installation
Run `npm install` to install the projects dependencies.

### Development Server
Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

### Build
Run `ng build --prod` for a production build of the project. The build artifacts will be stored in the `dist/UPT-GUI` directory.

### Deploy to Oskari (requires build)
**Disclaimer:** This code has only been tested with Oskari 1.54.

- After building the app, copy the `dist/UPT-GUI/` contents into `/Oskari${path}` in your server. If you're unsure of the path that `/Oskari${path}` refers to in the server, please visit [this link](https://github.com/oskariorg/sample-configs/blob/master/nginx/conf.d/default.conf) for help.
- From the `docs/index.html` file, copy the `<style>` element that contains an `href` similar to `styles.yyyyyyyyyyyyyyyy.css` and all the `<script>` elements within the `<body>` tag except the one that contains `scripts` in its `href` and add them into the `UPT-Server-Extension/webapp-map/src/main/webapp/WEB-INF/jsp/geoportal.jsp` file, adding to their respective `src` and `href` the following `/Oskari${path}` to the start of the path.

## References
- [UPT-Server-Extension](https://github.com/UPTechMX/UPT-Server-Extension)
- [Angular Docs](https://angular.io/)
- [PrimeNG](https://primefaces.org/primeng/showcase/#/setup)
- [PrimeIcons](https://www.primefaces.org/showcase/ui/misc/primeicons.xhtml)
- [Angular MDBootstrap](https://mdbootstrap.com/docs/angular/)
- [Angular Material](https://material.angular.io/)
- [Font Awesome](https://fontawesome.com/)

## License
- [MIT License](/LICENSE.md)
- Copyright (c) 2020 CAPSUS S.C.

## Acknowledgements

We acknowledge the invaluable support of the [World Bank’s Trust Fund for Statistical Capacity Building](https://worldbank.org/) (TFSCB) in making this project. This tool was conceptualized at [City Planning Labs](https://collaboration.worldbank.org/content/sites/collaboration-for-development/en/groups/city-planning-labs.html) with the technical support from [SITOWise](https://www.sitowise.com/en). The tools were developed by [CAPSUS](http://capsus.mx/) and are maintained by [UPTech](http://up.technology/) and a community of developers.
