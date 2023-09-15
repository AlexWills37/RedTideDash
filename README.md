# Red Tide Dashboard

This is the frontend for a web-dashboard project that aggregates information on Florida's Red Tide phenomenon from
multiple online sources into a single, easy-to-use dashboard.

This is the final project for the Software Engineering course tought by Professor Tania Roy.
It was designed and made by [Philip Gray](https://github.com/philipgray), [Ferris Whitney](https://github.com/fwhitney), and me over the course of 8 weeks.

This repository in particular is a copy of the original project, which is no longer deployed for cost reasons. This version, however, is [deployed with GitHub Pages](https://alexwills37.github.io/RedTideDash/).

## Background

*From the website:*
```
Red tide, a harmful algae bloom that regularly occurs on the coasts of Florida,
creates toxic conditions that negatively impact the environment, marine animals,
and human health. It can ruin beach days and endanger animals that call the Florida
coasts their home. This dashboard is a collection of updated information to help
you stay up-to-date on the current status of red tide in Florida. 
```

For people in Florida who live by the coasts or may want to visit the beaches, knowing about and understanding the status of the environment
in real time is valuable, and this dashboard seeks to fulfil that goal.

## Features

- Current measurements of Red Tide in different areas (measured by cell counts of algae), sortable by county
- Relevant podcasts on Spotify to learn about Red Tide and the environment
- Graph with the frequency of Red Tide Tweets over time
  to model the times of the year when Red Tide is present
- Recent Tweets about Red Tide to see the current conversation
- Relevant YouTube videos on Red Tide and its health implications
- Chatboard to dicuss Red Tide and report its appearance in real time
- Navigation bar to help with usability
- Confetti effect if you fill in the textbox at the bottom of the website with `Climbing`

Most of these features are dependent on an operating backend server, which is currently not running.

## Connecting to the Backend
The URL for the backend server must be set up correctly
in [the database-api.service.ts file](./src/app/services/database-api.service.ts) of this project on **line 75**:
```
private backendApiEndpoint = '<backend URL>';
```

To connect the [GitHub Pages website](https://alexwills37.github.io/RedTideDash/) with the backend, the URL must be configured on the [`gh-pages` branch](https://github.com/AlexWills37/RedTideDash/tree/gh-pages)  of this repository, and then the website must be built to the `/docs` folder.

Alternatively, this repository can be cloned, and both servers (this one, and the backend server) can be run locally (as long as the URL is configured to connect to the local backend server).






## Angular
This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 13.3.0.

