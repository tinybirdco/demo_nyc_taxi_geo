# Front-end application

This folder contains all of the code to build the frontend of this demo.

The app uses [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/guides), a client-side JavaScript library for building web maps and web applications with Mapbox's modern mapping technology.

**You will need to create an access token to make API requests.**

![Taxi Map](../image.png)

## Deploying the app

Edit the `map.html` file to add your Mapbox GL access token and Tinybird token (lines 66 and 82, respectively).

Install the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension. To launch the local server, right click on the HTML file and click on "Open with Live Server".

## Key Features

1. Transform the lat and long into H3 indexes (hexagons) to plot on the map.

2. The color intensity of the hexagons indicates the number of rides in that area (i.e. the density).

3. The resolution of the hexagons changes when you zoom in or out.

4. The dropdowns let you switch between taxi pickup and dropoff locations and filter on different vendors.

5. In the bottom left, there some stats about each API request, including query latency (in the database), roundtrip latency (including the network), and more.