<p align="center"><img src="https://images.weserv.nl/?url=raw.githubusercontent.com/Kupuyc/Kupuyc/master/images/art/mac1.jpg&w=320&h=320&fit=cover&mask=circle&maxage=7d" alt="Intro funny picture"/></p>

<p align="center">
  <a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&duration=2000&pause=1500&color=2EA0D2&center=true&width=435&lines=15+years+of+front-end+development.;I've+seen+some...+code (>_<);A+lot+of+code.;And+it's+great!+%5Co%2F" alt="Typing SVG"/></a>
</p>

<p align="center">
  <a href="https://t.me/kupuyc"><img src="https://img.shields.io/badge/Telegram-@kupuyc-blue?style=for-the-badge&logo=telegram&labelColor=gray" alt="Badge: Telegram"/></a>
  <span>&nbsp;&nbsp;&nbsp;</span>
  <a href="https://discordapp.com/users/802953005838106665"><img src="https://img.shields.io/badge/Discord-Kupuyc%238730-blue?style=for-the-badge&logo=discord&labelColor=gray&logoColor=5880f2" alt="Badge: Discord"/></a>
  <span>&nbsp;&nbsp;&nbsp;</span>
  <a href="https://habr.com/ru/users/Kupyc/"><img src="https://img.shields.io/badge/Habrahabr-kupyc-blue?style=for-the-badge&logo=habr&labelColor=gray" alt="Badge: Habrahabr"/></a>
</p>

# About me
<p align="center"><img src="images/art/bughunting.png" alt="About funny picture"/></p>

<pre><code>let me: PersonDetails = {
  name: {
    first: 'Кирилл',
    surname: 'Петров',
    pronounce: 'Kirill Petrov'
  },
  education: {
    university: 'Ryazan State Radio Engineering University named after V. F. Utkin'
    level: '<a href="https://en.wikipedia.org/wiki/International_Standard_Classification_of_Education">ISCED 6</a>'
  },
  job: [{
    position: 'Senior front-end developer',
    role: 'Teamlead',
    from: new Date('2020-05-20T00:00:00Z'),
    details: '<a href="#backoffice-for-the-print-subscription-service">#job-it1</a>'
  }, {
    position: 'Software developer',
    role: 'Fullstack developer',
    from: new Date('2009-12-05T00:00:00Z'),
    to: new Date('2020-05-10T00:00:00Z'),
    details: '<a href="#legal-reference-system-garant">#job-garant</a>'
  }],
  petProjects: [{
    name: 'Eve Fleet Manager',
    description: 'Set of tools for Eve Online video game: analysis, statistics, helpers.'
    details: '<a href="#eve-fleet-manager">#pet-efm</a>'
  }],
  goals: [{
    type: 'optional',
    name: 'Rewrite pet project using new stack.'
  }],
}</code></pre>

# Projects
<p align="center"><img src="images/art/rocket.png" alt="Projects funny picture"/></p>

## Legal reference system "Garant"
The application provides an opportunity to get up-to-date information about the articles of laws, see specific changes, compare versions of documents, and access older versions.

The development of the project began in 2012. The goal was to develop a SPA that would fully replicate the functionality of the desktop application. It was an ambitious goal - in those days there were no such rich tools as there are now, and we had to deal with finicky browsers. I designed the architecture of the application and wrote the base components of the system. After that the team was expanded by two developers, together with whom we started to add business functions.

At the time I left the company, the application had more than 50 screens, 700+ classes and components, and was about 2 Mb of JavaScript code. It was an extremely interesting project and I was happy to hear that the company was going to rewrite the application using the latest stack. Even now it's going to be a fascinating piece of work.

### Stack & tech
Front end:
* **Sencha ExtJS 4**

Back end:
* **Python** on *facade-server* of application which interacts with data-server via CORBA interface
* **C++** on *data-server* for access to huge self-written database

### Gallery
||||
|:---:|:---:|:---:|
|<a href="images/projects/garant/main.png?raw=1"><img src="images/projects/garant/main_preview.png" alt="Main screen"/><br/>Main page</a>|<a href="images/projects/garant/search.png?raw=1"><img src="images/projects/garant/search_preview.png" alt="Search results"/><br/>Search results</a>|<a href="images/projects/garant/document.png?raw=1"><img src="images/projects/garant/document_preview.png" alt="Document screen"/><br/>Document</a>|
|<a href="images/projects/garant/document_toc.png?raw=1"><img src="images/projects/garant/document_toc_preview.png" alt="Document + TOC"/><br/>Document + TOC</a>|<a href="images/projects/garant/document_editions.png?raw=1"><img src="images/projects/garant/document_editions_preview.png" alt="Document + editions"/><br/>Document + editions</a>|<a href="images/projects/garant/compare_editions.png?raw=1"><img src="images/projects/garant/compare_editions_preview.png" alt="Compare of two editions"/><br/>Compare of two editions</a>|

## Backoffice for the print subscription service
The project of subscription access to printed materials: magazines, newspapers, booklets, almanacs, etc. Thousands of publications, hundreds of publishers, delivery to millions of subscribers through the infrastructure of post offices.

For such a business to work, it is necessary to connect all the components and provide all the representatives with the opportunity to publish their materials conveniently, giving them the opportunity to subscribe to them. The project implemented tools for publishers and managers so that the former can submit a request to place material and the latter can process it. The system also allows managers to edit directories and dictionaries, work with mailing lists, generate reports, financial documents and much more.

The project was implemented as part of a microservice architecture of more than 30 services, and the data were aggregated on two sites - separately for publishers and for managers. In recent months, work has been underway to migrate the sites from the legacy stack to new technologies using [Feature-Sliced Design](https://feature-sliced.design/), React 17, TypeScript, code generation based on OpenAPI specifications, Gitlab CI/CD with deploying to Kubernetes, and so on.

### Stack & tech
Front end:
* **React 0.13**, **Angular 1**
* **React 17**, **Redux Toolkit**, **TypeScript 4.7**

Back end:
* **Java 8**
* **Java 17**, **Kotlin**

## Eve Fleet Manager
EFM is a pet project (in private repo) for universe of the [Eve Online](https://www.eveonline.com/) - #1 space MMORPG. The project specialized in providing analytical tools for players:
* Battle analysis with the ability to build a detailed statistical picture of the clash of thousands of players with automatic analysis of damage and distribution of players on the sides of the conflict. Thanks to the successful architecture, these calculations were extremely fast, even on large amounts of data, on the order of 0.15-0.4 seconds. In gallery below you may see an example of a clash of 2300 players who lost 2600 ships.
* Campaign analysis - a higher point of view on mass clashes of players in hundreds solar systems during weeks and months (up to year) and ability to analyze the degree of involvement and losses at the level of alliances and coalitions. The result is a picture with hundreds of thousands of ships lost. In gallery below you may see an example of campaign which describes 5 month war between several coalitions with 154000 in total number of pilots, who lost ~414000 ships which equal ~232000 USD.
* Fleet Assistant - thanks to [Meteor](https://www.meteor.com/)'s feature of reactive updating on the client of the data being changed in MongoDB, a tool was implemented to display the full fleet composition in the web application. Any change in fleet in the game was almost instantly reflected in the application, which allowed to operate the fleet giving opportunities that have not been implemented in the game so far. Additional functionality in the form of statistics on losses (total number of losses, rate of loss, etc.) and damage caused by the fleet allowed the commander to make strategic decisions.
* Other little tools like board of two types timers, wormhole map, etc

### Stack & tech
Frontend:
* **Meteor 1.10**, **SCSS**, **[Materialize](https://materializecss.com/)**

Back end:
* **Meteor**, **WebSocket**, **[ESI API](https://esi.evetech.net/ui/)**
* **MongoDB 4.0**

### Gallery
||||
|:---:|:---:|:---:|
|<a href="images/projects/efm/main.png?raw=1"><img src="images/projects/efm/main_preview.png" alt="Main page"/><br/>Main page<br/>(0.7 MB)</a>|<a href="images/projects/efm/battlereports.png?raw=1"><img src="images/projects/efm/battlereports_preview.png" alt="Most viewed battle reports"/><br/>Most viewed battle reports<br/>(0.2 MB)</a>|<a href="images/projects/efm/battlereport_ships.png?raw=1"><img src="images/projects/efm/battlereport_ships_preview.png" alt="Battle report: ships tab"/><br/>Battle report: ships tab<br/>(4.8 MB)</a>|
|<a href="images/projects/efm/battlereport_timeline.png?raw=1"><img src="images/projects/efm/battlereport_timeline_preview.png" alt="Battle report: timeline tab"/><br/>Battle report: timeline tab<br/>(3.4 MB)</a>|<a href="images/projects/efm/battlereport_summary.png?raw=1"><img src="images/projects/efm/battlereport_summary_preview.png" alt="Battle report: summary tab"/><br/>Battle report: summary tab<br/>(1.2 MB)</a>|<a href="images/projects/efm/battlereport_organizations.png?raw=1"><img src="images/projects/efm/battlereport_organizations_preview.png" alt="Battle report: organizations tab"/><br/>Battle report: orgs tab<br/>(2.1 MB)</a>|
|<a href="images/projects/efm/battlereport_players.png?raw=1"><img src="images/projects/efm/battlereport_players_preview.png" alt="Battle report: players tab"/><br/>Battle report: players tab<br/>(2.7 MB)</a>|<a href="images/projects/efm/campaign_ships.png?raw=1"><img src="images/projects/efm/campaign_ships_preview.png" alt="Campaign: ships tab"/><br/>Campaign: ships tab<br/>(2.1 MB)</a>|<a href="images/projects/efm/campaign_groups.png?raw=1"><img src="images/projects/efm/campaign_groups_preview.png" alt="Campaign: ship groups tab"/><br/>Campaign: ship groups tab<br/>(0.7 MB)</a>|
|<a href="images/projects/efm/campaign_organizations.png?raw=1"><img src="images/projects/efm/campaign_organizations_preview.png" alt="Campaign: orgs tab"/><br/>Campaign: orgs tab<br/>(0.4 MB)</a>|<a href="images/projects/efm/campaign_charts.png?raw=1"><img src="images/projects/efm/campaign_charts_preview.png" alt="Campaign: charts tab"/><br/>Campaign: charts tab<br/>(0.7 MB)</a>|<a href="images/projects/efm/campaign_top_losses.png?raw=1"><img src="images/projects/efm/campaign_top_losses_preview.png" alt="Campaign: top losses tab"/><br/>Campaign: top losses tab<br/>(1.6 MB)</a>|

# Tech & skills
<p align="center"><img src="images/art/unstoppable.png" alt="Tech and skills funny picture"/></p>

|      | Name | Seniority | Latest usage |
| :--- | ---  | ---       | ---          |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-plain-wordmark.svg" width="48" height="48" alt="HTML logo"/> | HTML | <img src="https://img.shields.io/badge/Senior-15%20years-green?style=flat-square&labelColor=green&color=gray" alt="Senior"/> | now |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-plain-wordmark.svg" width="48" height="48" alt="CSS logo"/> | CSS | <img src="https://img.shields.io/badge/Senior-15%20years-green?style=flat-square&labelColor=green&color=gray" alt="Senior"/> | now |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-plain.svg" width="48" height="48" alt="JavaScript logo"/> | JavaScript | <img src="https://img.shields.io/badge/Senior-15%20years-green?style=flat-square&labelColor=green&color=gray" alt="Senior"/> | now |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-plain.svg" width="48" height="48" alt="TypeScript logo"/> | TypeScript | <img src="https://img.shields.io/badge/Senior-3%20years-green?style=flat-square&labelColor=green&color=gray" alt="Senior"/> | now |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original-wordmark.svg" width="48" height="48" alt="React logo"/> | React | <img src="https://img.shields.io/badge/Senior-4%20years-green?style=flat-square&labelColor=green&color=gray" alt="Senior"/> | now |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/redux/redux-original.svg" width="48" height="48" alt="Redux logo"/> | Redux | <img src="https://img.shields.io/badge/Senior-4%20years-green?style=flat-square&labelColor=green&color=gray" alt="Senior"/> | now |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/webpack/webpack-original.svg" width="48" height="48" alt="Webpack logo"/> | Webpack | <img src="https://img.shields.io/badge/Middle-6%20years-green?style=flat-square&labelColor=yellow&color=gray" alt="Middle"> | now |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/eslint/eslint-original.svg" width="48" height="48" alt="ESLint logo"/> | ESLint | <img src="https://img.shields.io/badge/Senior-6%20years-green?style=flat-square&labelColor=green&color=gray" alt="Senior"/> | now |
| <img src="images/icons/express.svg" width="48" height="48" alt="Express logo"/> | Express | <img src="https://img.shields.io/badge/Middle-5%20years-green?style=flat-square&labelColor=yellow&color=gray" alt="Middle"> | now |
| <img src="images/icons/api.svg" width="48" height="48" alt="REST API logo"/> | REST API | <img src="https://img.shields.io/badge/Senior-9%20years-green?style=flat-square&labelColor=green&color=gray" alt="Senior"/> | now |
| <img src="images/icons/openapi.svg" width="48" height="48" alt="OpenAPI logo"/> | OpenAPI | <img src="https://img.shields.io/badge/Senior-3%20years-green?style=flat-square&labelColor=green&color=gray" alt="Senior"/> | now |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" width="48" height="48" alt="Java logo"/> | Java | <img src="https://img.shields.io/badge/Junior-3%20years-green?style=flat-square&labelColor=red&color=gray" alt="Junior"> | now |
| <img src="images/icons/microservice.svg" width="48" height="48" alt="Microservices logo"/> | Microservices | <img src="https://img.shields.io/badge/Middle-5%20years-green?style=flat-square&labelColor=yellow&color=gray" alt="Middle"> | now |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/ubuntu/ubuntu-plain-wordmark.svg" width="48" height="48" alt="Ubuntu logo"/> | Ubuntu Linux | <img src="https://img.shields.io/badge/Middle-6%20years-green?style=flat-square&labelColor=yellow&color=gray" alt="Middle"> | now |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-plain-wordmark.svg" width="48" height="48" alt="Docker logo"/> | Docker | <img src="https://img.shields.io/badge/Middle-3%20years-green?style=flat-square&labelColor=yellow&color=gray" alt="Middle"> | now |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/gitlab/gitlab-plain-wordmark.svg" width="48" height="48" alt="Gitlab logo"/> | Gitlab CI/CD | <img src="https://img.shields.io/badge/Middle-3%20years-green?style=flat-square&labelColor=yellow&color=gray" alt="Middle"> | now |
| <img src="images/icons/sencha.svg" width="48" height="48" alt="Sencha logo"/> | ExtJS (3, 4) | <img src="https://img.shields.io/badge/Senior-9%20years-green?style=flat-square&labelColor=green&color=gray" alt="Senior"/> | 3 years ago |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-plain-wordmark.svg" width="48" height="48" alt="Node.js logo"/> | Node.js | <img src="https://img.shields.io/badge/Middle-8%20years-green?style=flat-square&labelColor=yellow&color=gray" alt="Middle"> | 2 years ago |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/meteor/meteor-plain-wordmark.svg" width="48" height="48" alt="Meteor logo"/> | Meteor | <img src="https://img.shields.io/badge/Senior-6%20years-green?style=flat-square&labelColor=green&color=gray" alt="Senior"/> | 2 years ago |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original-wordmark.svg" width="48" height="48" alt="Python logo"/> | Python | <img src="https://img.shields.io/badge/Middle-9%20years-green?style=flat-square&labelColor=yellow&color=gray" alt="Middle"> | 3 years ago |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-original-wordmark.svg" width="48" height="48" alt="MongoDB logo"/> | MongoDB | <img src="https://img.shields.io/badge/Middle-6%20years-green?style=flat-square&labelColor=yellow&color=gray" alt="Middle"> | 2 years ago |

# Statistics
<p align="center"><img src="images/art/skills.png" alt="Statistics funny picture"/></p>

<p align="center"><img src="images/metrics.svg" alt="Statistics: languages"/></p>