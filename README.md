# mappapp (V.1)

## Overview (V2)

The purpose of this web application is to provide a lay-of-the-land for the user of a local road-network.

### Use Case #1

1. The user wants to learn about the Santa Clara County area and its roads, ie when the roads are very busy and on what days.
1. The app will display a birds-eye-view of the area, allowing the user to navigate around and click a road.
1. The application will then display a popup detailing the traffic of that day, hour-by-hour for the current day.

### Use Case #2

1. The user wants to examine the traffic for all days of the week.
1. The user can select another day from a "day-picker" and examine the hourly traffic.

## Detailed Design

### Front End

- Using the [leaflet](https://leafletjs.com) open-source map builder to capture mouse events and output global coordinates, ie longitude and lattitude.
- We will use [React.js](https://reactjs.org) as our UI framework.

### Back End

- We will use [Python Flask](https://flask.palletsprojects.com/en/2.0.x/) for our web framework.
- We will use [Inrix](https://inrix.com)'s API to access live and predicted traffic data on queried global coordinates.