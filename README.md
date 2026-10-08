# ⚡ EV Charging Stations in Nagpur — Power BI Dashboard

An interactive **Power BI dashboard for exploring EV charging stations across Nagpur, Maharashtra**.

The dashboard is designed to help EV users quickly identify charging stations, understand their charging capabilities, and inspect station-level information such as connector types, charging speed, available connectors, operating hours, ratings, and location.

---

## 📊 Dashboard Preview

### Station Overview & Map

![EV Charging Stations in Nagpur](assets/ev-charging-dashboard-1.png)

### Station Details

![EV Charging Station Details](assets/ev-charging-dashboard-2.png)

> **Note:** Add the two dashboard screenshots to an `assets` folder using the filenames shown above.

---

## 🎯 Project Objective

The objective of this project is to build an interactive and user-friendly **EV charging station locator and information dashboard** for Nagpur.

Instead of looking through raw charging-station data, users can interact with the dashboard to:

- Explore charging stations geographically
- Select an individual charging station
- View detailed station information
- Understand available connector types
- Check charging speed and available connectors
- View charging capacity information
- Check station ratings
- View station address and operating hours
- Identify stations operating 24 hours

---

## 🚀 Key Features

### 🗺️ Interactive Charging Station Map

The dashboard includes an interactive map showing the geographical distribution of EV charging stations across Nagpur.

Users can select a station directly from the map and view its corresponding details.

### 🔌 Connector Information

For the selected station, the dashboard displays available connector types such as:

- CCS
- Type 6
- Wall Socket
- Other available connector types depending on the station

Connector images are displayed to make the information easier to understand.

### ⚡ Charging Information

The dashboard provides station-level charging information including:

| Metric | Description |
|---|---|
| kWh | Charging capacity/energy information |
| Speed | Charging speed such as Fast |
| Connectors | Number of available connectors |
| Connector Type | Type of EV connector supported |

### ⭐ Station Rating

Each selected station displays its available rating on a 5-point scale.

### 📍 Location Details

The dashboard provides the complete address of the selected charging station and connects it with the map location.

### 🕐 Operating Hours

Users can view the operating days and hours of the selected charging station, including stations operating **24 hours**.

### 🔄 Interactive Station Selection

Selecting a station updates the relevant:

- Station image
- Map location
- Charging metrics
- Connector information
- Address
- Operating hours
- Rating

This creates a single interactive experience rather than a static report.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard development and visualization |
| **Power Query (M)** | Data transformation and preparation |
| **DAX** | Measures, calculations and dynamic dashboard logic |
| **EV Charging Data / API** | Charging-station information |
| **Map Visual** | Geographical station visualization |
| **HTML / Custom Visual Elements** | Enhanced station cards and UI presentation |

---

## 🔄 Data & Dashboard Workflow

```text
EV Charging Station Data
          │
          ▼
     Power Query
          │
          ▼
 Data Cleaning & Transformation
          │
          ▼
     Data Modeling
          │
          ▼
      DAX Measures
          │
          ▼
 Interactive Power BI Dashboard
          │
     ┌────┴────┐
     ▼         ▼
    Map    Station Details
     │         │
     └────┬────┘
          ▼
  Interactive User Experience
