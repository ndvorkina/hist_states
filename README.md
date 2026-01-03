# Historical States Database 🌍📜
List of all states in world history

## 📖 Overview
This repository contains a structured bilingual (English/Russian) dataset for an **interactive historical atlas** application. The data chronicles sovereign states, empires, and political entities from antiquity to the modern era, designed to visualize the dynamic nature of geopolitical borders and historical transformations.

The core purpose of this dataset is to serve as a backend for providing essential contextual information for each state.

## 🗃️ Dataset Structure
### 1. General Interface and System Fields
These fields define the **UI elements, titles, and system-wide labels** used throughout the application:

*   **`titleAttr`**: The main descriptive attribute for the atlas (e.g., "World History Atlas | Ancient and Modern States").
*   **`mainTitle`** and **`title`**: The primary headings displayed to the user, such as "Historical Map".
*   **`labels`**, **`states`**, and **`events`**: Identifiers for the different categories of information displayed on the map.
*   **`source`** / **`data`**: Used to credit the data source.
*   **`feedback`** / **`mail`**: Contact points for user communication.
*   **`year`**, **`time`**, and **`dates`**: Variables used to manage the temporal navigation of the map.
*   **`out`**: A status indicator for objects currently outside the user's field of view.
*   **`dateTooltip`**: Text for the hover-over element explaining border changes.
*   **`label_empty`**: A placeholder used to indicate that a specific section is "under construction".
*   **`label_uninhabited`**: A specific label identifying territories that were uninhabited during a given period.

### 2. Historical Entity Fields (Numbered Data)
For every historical state, empire, or city-state, the sources use a **standardized numbering system** (where `i` represents a unique index, such as `name_1`, `name_2`, etc.):

*   **`name_i`**: The full official name of the historical entity (e.g., "Troy", "Hittite Kingdom", "Achaemenid Empire").
*   **`capital_i`**: The name of the capital city or cities associated with that entity.
*   **`label_i`**: A shortened version of the name intended for display directly on the map surface.
*   **`info_i`**: A comprehensive historical summary. Based on the sources, this field consistently includes:
    *   **Dates of existence** (e.g., "3000–1260 BC").
    *   **Type of state** (e.g., "slave-owning", "monarchical", "feudal").
    *   **Geographic origin** (e.g., "territory of modern Turkey" or "modern Iraq").
    *   **Cause of collapse** (e.g., "Conquered by Assyria" or "Destroyed by ancient Greeks").
    *   **Notable rulers** (where applicable, such as Cyrus II or Alexander the Great).

## 🌍 Scope & Coverage
The dataset aims for broad historical and geographical coverage:

*   **Chronological Span:** From ancient civilizations (e.g., **Assyria**, **Maurya Empire**, **Maya**) to contemporary nations (e.g., **Turkey**, **Poland**, **post-Soviet states**).
*   **Political Diversity:** Includes empires, kingdoms, republics, confederacies, and other sovereign entities.
*   **Key Processes:** Special attention is given to:
    *   The **colonial possessions** of major empires (British, French, Spanish, etc.).
    *   The **decolonization** and independence movements of the 20th century.
    *   Major geopolitical shifts (dissolutions, unifications, Successor states).

## 🛠️ Technical Implementation
*   **Format:** The data is structured in a machine-readable format (e.g., JSON, XLSX) for easy integration.

## 🎯 Primary Use Case
To power an interactive application that allows users to:
1.  Temporal data organization for timeline visualization
2.  Observe the **rise and fall of states** and the **shifting of borders**.
3.  Click on any polity to view its **core metadata** (name, capital, historical summary).

*   **Contributions:** Feedback, corrections, and suggestions for new entries are welcome. Please open an **Issue** or **Pull Request** for substantive changes.

The repository contains:
- States.xlsx - by Dvorkin Boris and Elena
- en.json, ru.json - used in [worldhist.org](https://worldhist.org)
