# Tribal Agriculture Management Portal

A browser-based portal for managing tribal agriculture information,
farmer records, crop details, land-area summaries, and government scheme
updates.

## Features

### Login and user roles

-   Separate login options for **Farmer** and **Agriculture Officer**.
-   Role-based interface visibility.
-   Demo credentials are displayed on the login screen:
    -   **Officer:** `officer` / `officer123`
    -   **Farmer:** `farmer` / `farmer123`

### Dashboard

-   Summary of total farmers, crop records, total crop area, and active
    schemes.
-   Displays the three most recently updated government schemes.
-   Shows crop-wise area totals and relative shares.

### Farmer management

-   Officers can register farmers with name, village, mobile number, and
    land owned.
-   Farmer records are displayed in a table.
-   The Settings page lets users show or hide optional farmer-table
    columns: village, mobile, land owned, and crops grown.

### Crop management

-   Add crop records by selecting a farmer and entering the crop name,
    area in acres, and season.
-   Supported seasons: Kharif, Rabi, and Summer.
-   View crop records and crop-wise area summaries.
-   The portal warns if the entered crop area exceeds the farmer's
    recorded land area; the user can choose whether to continue.

### Land map

-   Select a farmer to view their recorded land owned, area under crops,
    and remaining land.
-   An embedded Google Map displays the selected farmer's village
    location.
-   **Note:** The map currently shows the village location, not surveyed
    plot boundaries. Exact plot mapping would require plot coordinates
    or boundary data. An internet connection is required for the
    embedded map.

### Government schemes

-   Officers can add a scheme or update an existing scheme with the same
    name.
-   Scheme details include benefit, description, and status (Active or
    Closed).
-   Saved schemes are displayed in the Government Schemes section and on
    the dashboard.

### Settings and support

-   Configure which optional columns appear in the farmer table.
-   Support contact details are displayed in the Settings section.

## Getting started

### Requirements

-   A modern web browser (such as Chrome, Edge, Firefox, or Safari).
-   Internet access for the embedded Google Map.

### Run locally

1.  Download or copy `index.html` to your computer.
2.  Open the file in a web browser.
3.  Choose a role on the login screen.
4.  Enter one of the demo usernames and passwords listed above.

No package installation, build process, or backend server is required
for the current standalone version.

## Project structure

``` text
.
└── index.html   # Complete website: HTML, CSS, and JavaScript
```

The page contains the interface markup, styling, sample data, and
application logic in one HTML file.

## Sample data

The website starts with sample farmer, crop, and government-scheme
records so that the dashboard and tables are populated when opened.
These records are defined in the JavaScript section of `index.html`.

## Important implementation notes

-   **Demo authentication only:** The current login checks fixed
    usernames and passwords in client-side JavaScript. It is suitable
    for demonstration, not real-world account security.
-   **No persistent database:** Farmer, crop, and scheme changes are
    held in browser memory while the page is open. Reloading the page
    resets the data to the original sample records.
-   **No server-side authorization:** Hiding or showing interface
    sections based on a selected role is not a secure access-control
    system.
-   **Map precision:** The map is searched using the farmer's village
    name in Andhra Pradesh. It does not identify the farmer's exact land
    parcel.
-   **Scheme verification:** Users should confirm scheme eligibility,
    benefits, deadlines, and current availability with the relevant
    government department.

## Suggested improvements for production use

1.  Add secure authentication and server-side role permissions.
2.  Connect the portal to a database with reliable data storage and
    backups.
3.  Add input validation, audit logs, and controlled access to personal
    information.
4.  Store verified GPS coordinates and surveyed land boundaries for
    accurate plot mapping.
5.  Add tests, error handling, and deployment configuration.

## Support

The website currently displays the following support details in its
Settings section:

-   **Email:** killojayanthi734@gmail.com
-   **Phone:** 8331056252
-   **Location:** Sundruputtu, Paderu, ASR District, Andhra Pradesh

------------------------------------------------------------------------

© 2026 Tribal Agriculture Management Portal
# tribal-agriculture-management-portal
