# Burkina Faso Conflict Map (2018–2023)

## Interactive Visualization of Conflict Events

This project presents an **interactive map visualization of conflict events in Burkina Faso from 2018 to 2023**.  
The map displays the **location and severity of attacks over time**, allowing users to explore how conflict evolves geographically and temporally.

The visualization is built using **Mapbox GL JS** and a **GeoJSON dataset**, with an animated timeline that cycles through years.

---

## Project Overview

Understanding the **spatial and temporal dynamics of conflict** is important for researchers, policymakers, and analysts studying security and political stability.

This project provides an **interactive visualization tool** that allows users to:

- explore where attacks occurred
- see how conflict intensity changes over time
- identify geographic hotspots
- observe the spread of violence across regions

The map includes:

- an **interactive timeline slider**
- **automatic animation** of conflict events over time
- **visual encoding of attack severity** through circle size and color

---

## Features

### Interactive Map

The map displays conflict events using **geographic coordinates from a GeoJSON dataset**.

Each event is represented as a **circle marker** on the map.

---

### Timeline Animation

The visualization includes a **timeline slider covering the years 2018–2023**.

Users can:

- manually select a year
- play an animation showing how events evolve over time

---

### Severity Visualization

Conflict intensity is visualized using two encodings:

**Circle size**

The radius of each circle increases with the number of fatalities.

**Circle color**

Color intensity also reflects the number of fatalities.

- Low fatalities → light pink  
- High fatalities → dark red

---

## Technologies Used

This project uses the following technologies:

- **Mapbox GL JS** – interactive map rendering
- **GeoJSON** – spatial data format
- **JavaScript** – map animation and filtering
- **HTML / CSS** – web interface

---

## Dataset Structure

The map loads a GeoJSON file containing conflict events.

Each event includes attributes such as:

- geographic coordinates
- year of the event
- number of fatalities

Example structure:

```json
{
  "type": "Feature",
  "properties": {
    "year": 2019,
    "fatalities": 12
  },
  "geometry": {
    "type": "Point",
    "coordinates": [-2.45, 12.37]
  }
}
