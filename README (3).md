# ⚡ EV Charging Stations in Nagpur --- Power BI Dashboard

An interactive **Power BI dashboard for exploring EV charging stations
across Nagpur, Maharashtra**.

The dashboard is designed to help EV users quickly identify charging
stations, understand their charging capabilities, and inspect
station-level information such as connector types, charging speed,
available connectors, operating hours, ratings, and location.

------------------------------------------------------------------------

## 📊 Dashboard Preview

### Station Overview & Map

![EV Charging Stations in Nagpur](assets/ev-charging-dashboard-1.png)

### Station Details

![EV Charging Station Details](assets/ev-charging-dashboard-2.png)

> **Note:** Add the two dashboard screenshots to an `assets` folder
> using the filenames shown above.

------------------------------------------------------------------------

## 🎯 Project Objective

The objective of this project is to build an interactive and
user-friendly **EV charging station locator and information dashboard**
for Nagpur.

Instead of looking through raw charging-station data, users can interact
with the dashboard to:

-   Explore charging stations geographically.
-   Select an individual charging station.
-   View detailed station information.
-   Understand available connector types.
-   Check charging speed and available connectors.
-   View estimated/recorded charging capacity in kWh.
-   Check station ratings.
-   View station address and operating hours.
-   Identify stations that are open 24 hours.

------------------------------------------------------------------------

## 🚀 Key Features

### 🗺️ Interactive Charging Station Map

The dashboard includes an interactive map showing the geographical
distribution of EV charging stations across Nagpur.

Users can select a station directly from the map and view its
corresponding details.

### 🔌 Connector Information

For the selected station, the dashboard displays available connector
types such as:

-   CCS
-   Type 6
-   Wall Socket
-   Other available connector types depending on the station

Connector images are displayed to make the information easier to
understand.

### ⚡ Charging Information

The dashboard provides station-level charging information including:

  -----------------------------------------------------------------------
  Metric                              Description
  ----------------------------------- -----------------------------------
  kWh                                 Charging capacity/energy
                                      information available for the
                                      selected station

  Speed                               Charging speed such as Fast

  Connectors                          Number of available connectors

  Connector Type                      Type of EV connector supported
  -----------------------------------------------------------------------

### ⭐ Station Rating

Each selected station displays its available rating on a 5-point scale.

### 📍 Location Details

The dashboard provides the complete address of the selected charging
station and connects it with the map location.

### 🕐 Operating Hours

Users can view the operating days and hours of the selected charging
station, including stations operating **24 hours**.

### 🔄 Interactive Station Selection

The dashboard is designed around cross-filtering. Selecting a station
updates the relevant:

-   Station image
-   Map location
-   Charging metrics
-   Connector information
-   Address
-   Operating hours
-   Rating

This creates a single interactive experience rather than a static
report.

------------------------------------------------------------------------

## 🛠️ Tech Stack

  -----------------------------------------------------------------------
  Technology                          Purpose
  ----------------------------------- -----------------------------------
  **Power BI Desktop**                Dashboard development and
                                      visualization

  **Power Query (M)**                 Data transformation and preparation

  **DAX**                             Measures, calculations and dynamic
                                      dashboard logic

  **EV Charging Data / API**          Charging-station information

  **Map Visual**                      Geographical station visualization

  **HTML / Custom Visual Elements**   Enhanced station cards and UI
                                      presentation
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## 🔄 Data & Dashboard Workflow

The overall workflow of the project is:

``` text
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
```

------------------------------------------------------------------------

## 🧹 Data Preparation

The raw charging-station data was prepared before visualization.

Typical preparation steps included:

-   Removing unnecessary columns.
-   Handling missing values.
-   Standardizing station names.
-   Cleaning address information.
-   Formatting latitude and longitude fields.
-   Preparing connector information.
-   Structuring charging-speed and connector fields.
-   Creating fields required for map visualization.
-   Preparing station-level attributes for dynamic display.

Power Query was used to perform the required transformations before
loading the data into the Power BI model.

------------------------------------------------------------------------

## 📐 Power BI & DAX

DAX was used to create dynamic calculations and support the interactive
station-selection experience.

The dashboard uses measures and calculated logic to dynamically display
information for the selected charging station.

Examples of dashboard metrics include:

``` text
Selected Station
Available Connectors
Charging Capacity
Charging Speed
Station Rating
Operating Hours
Station Address
```

The combination of **DAX + Power BI interactions + map selection**
allows the dashboard to update based on the user's selected station.

------------------------------------------------------------------------

## 🎨 Dashboard Design

The dashboard uses a dark, high-contrast visual theme with bright accent
colors to create an EV/technology-oriented interface.

### Main layout

**Top section** - Dashboard title - Selected station image - Station
rating - Connector availability

**Middle section** - Interactive charging-station map - Charging
information cards

**Bottom section** - Connector type information - Connector images -
Detailed station information - Address - Operating hours - Rating

The layout was designed to keep the most important information visible
without requiring users to navigate through multiple report pages.

------------------------------------------------------------------------

## 🔍 Example User Flow

A typical user interaction looks like this:

``` text
Open Dashboard
      ↓
Explore charging stations on map
      ↓
Select a charging station
      ↓
Station details update automatically
      ↓
Check charging speed
      ↓
Check connector availability
      ↓
View connector type
      ↓
Check address & operating hours
      ↓
Compare/select a suitable station
```

------------------------------------------------------------------------

## 📌 Example Station Information

For a selected station, the dashboard can display information such as:

``` text
Station:
Electric Vehicle Charging Station

Location:
Airport Metro Station, Sonegaon,
Nagpur, Maharashtra 440005

Charging Speed:
Fast

Connectors:
4

Operating Hours:
Open 24 hours

Rating:
4 / 5
```

The values shown above are examples from the dashboard preview and can
change depending on the selected station.

------------------------------------------------------------------------

## 📁 Suggested Repository Structure

``` text
EV-Charging-Stations-Nagpur/
│
├── README.md
│
├── PowerBI/
│   └── EV_Charging_Stations_Nagpur.pbix
│
├── assets/
│   ├── ev-charging-dashboard-1.png
│   └── ev-charging-dashboard-2.png
│
└── data/
    └── README.md
```

> If the original charging-station dataset/API data cannot be
> redistributed, do not upload restricted or proprietary raw data.
> Instead, document the data source and setup process.

------------------------------------------------------------------------

## 💡 Business Value

The dashboard demonstrates how location-based EV infrastructure data can
be converted into an interactive analytical product.

Potential use cases include:

-   **EV drivers** --- finding suitable charging stations.
-   **Charging-network operators** --- understanding station
    distribution.
-   **Infrastructure planners** --- identifying areas with charging
    coverage.
-   **Businesses** --- analyzing charging infrastructure availability.
-   **Urban planners** --- supporting EV infrastructure expansion
    decisions.

------------------------------------------------------------------------

## 📈 Future Enhancements

Possible improvements for future versions include:

-   🔋 Real-time charger availability.
-   💰 Charging cost estimation.
-   🚗 EV-model compatibility.
-   ⏱️ Estimated charging time.
-   📍 Nearest charging station based on user's location.
-   🛣️ Distance and route calculation.
-   📊 Station utilization analysis.
-   📅 Historical charging trends.
-   🔔 Charger availability alerts.
-   🌐 Expansion to other cities in Maharashtra.
-   📱 Mobile-friendly dashboard design.

------------------------------------------------------------------------

## 🧠 What This Project Demonstrates

This project showcases practical skills in:

-   **Power BI**
-   **Power Query**
-   **DAX**
-   **Data Cleaning**
-   **Data Modeling**
-   **Interactive Data Visualization**
-   **Geospatial Visualization**
-   **API/Data Integration**
-   **Dashboard UI/UX**
-   **Business Intelligence**
-   **Analytical Storytelling**

------------------------------------------------------------------------

## 👨‍💻 Author

**Jaykumar Kadao**

Data Analyst \| Power BI \| SQL \| Python \| Data Visualization

------------------------------------------------------------------------

## ⭐ If You Like This Project

If this project helped you or you found it interesting, consider giving
the repository a ⭐ on GitHub.
