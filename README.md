<!--
![dsc banner](/images/dsc-banner5-white.png "DSC Banner")

# [DSC UTP](dscutp.github.io)
Official website for the DSC UTP (Developer Student Clubs Universiti Teknologi PETRONAS)

Developer Student Clubs (DSC) are community groups for students from any academic background in their undergraduate or graduate term. By joining a DSC, students build their professional and personal network, get access to Google developer resources, and work together to build solutions for local problems in a peer-to-peer learning environment.

## Installation
The website is built with jekyll, hence jekyll and ruby need to be installed for development.
- [Install Jekyll and ruby](https://jekyllrb.com/docs/installation/)

After installing jekyll, you can proceed to clone the project:
```
$ git clone https://github.com/dscutp/dscutp.github.io.git
```

## Run
To run the website, use the following command in the root directory of the project:
```
$ bundle exec jekyll serve
```
Note: just running `$ jekyll serve`  command is enough sometimes depending your installation

The website will run on port 4000 by default, open `localhost:4000` on your browser to see the website.

## Development
-->

<!--
*** Thanks for checking out this README Template. If you have a suggestion that would
*** make this better, please fork the repo and create a pull request or simply open
*** an issue with the tag "enhancement".
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
<p align="center">
  <a href="https://github.com/dscutp/dscutp.github.io">
    <img src="/images/dsc-banner5-white.png" alt="Logo" width="600">
  </a>

  <h3 align="center">DSC UTP</h3>

  <p align="center">
    Official website for DSC UTP (Developer Student Clubs UTP)
    <br />
    <a href="https://github.com/dscutp/dscutp.github.io"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://dscutp.com/">View Demo</a>
    ·
    <a href="https://github.com/dscutp/dscutp.github.io/issues">Report Bug</a>
    ·
    <a href="https://github.com/dscutp/dscutp.github.io/issues">Request Feature</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
  * [Built With](#built-with)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
* [Documentation](#documentation)
  * [Index Page](#index-page)
  * [Team Member](#team-member)
    * [Adding a Member/Changing Details](#adding-a-member/changing-details)
    * [Change Styling](#change-styling)
  * [Activity/Event](#activity/event)
    * [Adding New Activity](#adding-new-activity)
    * [Changing Page Layout](#changing-activity/event-page-layout)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#contact)
* [Acknowledgements](#acknowledgements)



<!-- ABOUT THE PROJECT -->
## About The Project

Developer Student Clubs (DSC) are community groups for students from any academic background in their undergraduate or graduate term. By joining a DSC, students build their professional and personal network, get access to Google developer resources, and work together to build solutions for local problems in a peer-to-peer learning environment.

### Built With

* [MDBootstrap](https://mdbootstrap.com/)
* [JQuery](https://jquery.com)
* [Jekyll](https://jekyllrb.com/)



<!-- GETTING STARTED -->
## Getting Started

### Prerequisites

The website is built with jekyll, hence jekyll and ruby need to be installed for development.
- [Install Jekyll and ruby](https://jekyllrb.com/docs/installation/)



### Installation

After installing jekyll, you can proceed to clone the project:
```
$ git clone https://github.com/dscutp/dscutp.github.io.git
```

To run the website, use the following command in the root directory of the project:
```
$ bundle exec jekyll serve
```
Note: just running `$ jekyll serve`  command is enough sometimes depending your installation

The website will run on port 4000 by default, open `localhost:4000` on your browser to see the website.



<!-- USAGE EXAMPLES -->
## Documentation

The structure of the project looks something like this:
```
.
├── _config.yml
├── _data
|   └── team.yml
├── _posts # currently where activity posts is stored
|   └── 2019-10-05-git-and-github-workshop.md
├── _includes
|   ├── events.html # Show activities card list
|   ├── footer.html
|   ├── head.html # head tag of the site
|   ├── navigation.html # Navigation bar and stuff
|   ├── preloader.html # show google preloader
|   └── team.html # show core team member card list
├── _layouts
|   ├── default.html # Layout of root page
|   └── post.html # Layout of activity/post page
├── _assets # put images/assets for post/activity here_
├── _images # put all other images here
├── _css
├── _js
├── _site # Dont touch this folder, it should be regenerated by jekyll
└── index.html # Root page of this folder
```

### Index Page
To make changes on the index page, go to `index.html` in the root directory. Do note that some part have been modularized and separatated into files in `_includes` directory. Also, the `index.html` is using `_layouts/default.html` layout.

### Team Members
This section covers making change on Team sections shown on the root page.
#### Adding a member/Change details
Go to `data/team.yml`, and make the necessary change
#### Changing Styling
Go to `_includes/team.html` to make changes on the html code of the Team section.

### Activity/Event
This section covers making change on Activity/Event sections on the root page.
#### Adding New Activity
Create a new file inside `_posts` directory. Please follow the naming convention `YYYY-MM-DD-title-of-event.md`. A HTML file may be used instead of markdown.

Inside the file, the following front matter can be used.
```
---
layout: post
title:  "Title of Workshop"
date:   2019-10-05 15:54:18 +0800 # Date of posting
categories: event
event_date: 2019-10-23 08:00:00 +0800 # Date of the event (will be shown on card)
thumbnail: assets/thumbnail-file-name.jpg
---
```
Please upload the thumbnail of the event inside `assets` directory, and put the thumbnail path on the front matter.

#### Changing Activity/Event Page layout
The HTML code used for the event page can be changed in the `_layouts/post.html`. If you want to use a unique layout instead, create a new html file inside `_layouts` directory. Then specify the use the created layout on the front matter of the post.



<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/othneildrew/Best-README-Template/issues) for a list of proposed features (and known issues).



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project / Clone the project (For members that have been given access)
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

You can message us on our [Facebook Page](https://www.facebook.com/dscutp/).




<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)





<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=flat-square
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=flat-square
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=flat-square
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=flat-square
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=flat-square
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png




