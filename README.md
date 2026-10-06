# Maclyn Outdoors

### Outdoor Intelligence
**Know. Decide. Go.**

Maclyn Outdoors is an outdoor intelligence platform I am designing and developing to help hunters and outdoor enthusiasts turn environmental data into simple, useful decisions in the field.

The project combines a Flutter-based mobile application with Garmin Connect IQ applications. It brings together location, weather, solar, lunar, and hunting-related information and transforms those inputs into practical information that can be quickly understood outdoors.

This repository is a public portfolio and project overview. The production source code is maintained in private repositories.

## Screenshots

### Maclyn Mobile

<img width="362" height="453" alt="View recent photos 4" src="https://github.com/user-attachments/assets/1989abe8-e8ac-4c15-8b49-19f99f3f5a35" />


<img width="316" height="405" alt="View recent photos 2" src="https://github.com/user-attachments/assets/54b3fbcd-044b-4441-a19c-34198ee12411" />



### Garmin Connect IQ

<img width="480" height="528" alt="View recent photos" src="https://github.com/user-attachments/assets/8f091908-5d89-4a1e-93af-81c091150e77" />

<img width="353" height="508" alt="View recent photos 3" src="https://github.com/user-attachments/assets/61b82f5e-08d1-40fc-97d9-539c62f91908" />


---

## Why I Built Maclyn

Hunters and outdoor enthusiasts often rely on several different sources of information before heading into the field:

- Weather conditions
- Sunrise and sunset
- Legal hunting light
- Wind speed and direction
- Moon phase and illumination
- GPS/location information
- Forecast conditions
- Field planning information

The goal of Maclyn is not simply to display more data.

The goal is to take available data, validate it, perform useful calculations, and present the results in a way that helps someone answer a much simpler question:

**What do I need to know before I go?**

---

## Current Platform

Maclyn currently includes development across two primary platforms.

### Maclyn Mobile

A Flutter/Dart mobile application designed to provide detailed outdoor intelligence and planning tools.

Current and developing features include:

- Sunrise and sunset calculations
- Legal hunting-light calculations
- Daylight remaining
- Weather conditions and forecasts
- Wind speed, direction, and gusts
- Moon phase and illumination
- Location-based environmental information
- Saved/custom locations
- Night Before Planner
- Hunting-time analysis
- GPS and mapping functionality
- Garmin integration

### Garmin Connect IQ

Maclyn also includes Garmin Connect IQ applications designed to put important field information directly on compatible Garmin watches.

Development includes:

- Maclyn Outdoor Watch
- Maclyn Outdoor Widget
- Sunrise and sunset
- Legal hunting-light windows
- Daylight remaining
- GPS status and location age
- Battery-conscious data handling
- Multiple hunting/legal-light modes
- Support for multiple Garmin display sizes and device families

The Garmin applications are developed using Monkey C and Garmin Connect IQ.

---

## Technologies

### Mobile Development
- Flutter
- Dart
- Android

### Garmin Development
- Garmin Connect IQ
- Monkey C

### Data & Integration
- REST APIs
- JSON
- GPS/location data
- Weather data
- Solar data and calculations
- Lunar data and calculations
- Persistent application data
- Data transformation
- Data validation

### Development Workflow
- Git
- GitHub
- VS Code
- Android Studio
- Garmin Connect IQ SDK
- AI-assisted development and debugging

---

## Data Flow

A simplified Maclyn data workflow looks like this:

**Location / GPS / API Data**  
↓  
**JSON / Structured Data**  
↓  
**Validation & Error Handling**  
↓  
**Application Logic & Calculations**  
↓  
**Derived Outdoor Metrics**  
↓  
**Mobile / Garmin User Interface**

The application does more than display raw API responses. Incoming information must be checked, transformed, combined with application logic, and converted into values that are useful to the user.

---

## Data Quality & Validation

One of the most important lessons from developing Maclyn has been that receiving data does not necessarily mean the data is correct or useful.

Development has required identifying and troubleshooting issues involving:

- Missing data
- Stale location information
- Incorrect time calculations
- Time and date handling
- Location-dependent calculations
- Unexpected API responses
- Data persistence
- Inconsistent calculated values
- Device-specific behavior

For example, solar information must be evaluated using the correct location, date, and time assumptions before sunrise, sunset, or legal hunting-light information can be trusted.

These problems have made data validation and testing a significant part of the development process.

---

## Turning Data Into Decisions

A core design principle behind Maclyn is that users should not have to interpret large amounts of raw information while preparing for or participating in an outdoor activity.

Maclyn therefore focuses on converting data into decision-oriented information.

Instead of simply presenting a sunrise value, for example, the application can use solar information and hunting rules to calculate:

- Legal hunting start time
- Legal hunting end time
- Time until legal light
- Remaining legal hunting time
- Remaining daylight

This same approach is being expanded into weather, hunting-time analysis, and field planning.

---

## Example Problem: Location Data

Outdoor applications cannot always assume that current GPS information is available.

Maclyn therefore has to account for situations such as:

- Missing GPS data
- Previously stored locations
- Aging location information
- Significant movement between locations
- Device GPS limitations

The Garmin applications include logic for tracking location information and communicating GPS status to the user rather than silently treating potentially stale information as current.

---

## Example Problem: Cross-Platform Development

Maclyn is being developed across devices with significantly different capabilities.

A modern Android phone can process and display considerably more information than an older Garmin outdoor watch.

The Garmin implementation therefore requires attention to:

- Memory constraints
- Battery consumption
- Screen size
- Display technology
- GPS availability
- Data caching
- Update frequency
- Device compatibility

The project uses the Garmin Fenix 5X as a baseline for maintaining compatibility with older supported hardware while expanding toward newer Garmin devices.

---

## Product Development

Maclyn is an active development project rather than a coding exercise.

Development includes:

- Identifying user problems
- Designing features
- Writing and integrating application logic
- Testing calculations
- Troubleshooting errors
- Collecting tester feedback
- Improving the user interface
- Supporting multiple devices
- Maintaining existing functionality while adding features

Real-world field testing has helped identify usability and data issues that are difficult to discover through development tools alone.

---

## Background

Maclyn also represents my return to hands-on technology and data work.

Earlier in my career at HomeAdvisor, I worked with SQL, Excel reporting, quality assurance, business analysis, and enterprise data processes. I also completed Level 1 Informatica training/certification in 2012.

My career later shifted toward ministry, education, and nonprofit leadership.

Developing Maclyn has allowed me to combine that earlier analytical background with modern application development, APIs, structured data, version control, testing, and data-quality practices.

I am continuing to strengthen my skills in data analytics, application development, and modern data tools.

---

## Current Development Areas

Current and planned Maclyn development includes:

- Expanded weather intelligence
- Hunting-time analysis
- Historical condition comparison
- Trail-camera data analysis
- GPS mapping
- GPX support
- Garmin/mobile synchronization
- Expanded Garmin device compatibility
- iOS support
- Improved data visualization and progressive disclosure

---

## Repository Structure

The production Maclyn source code is maintained in private repositories.

This public repository is intended to document:

- Project architecture
- Technical decisions
- Data workflows
- Screenshots
- Development milestones
- Selected non-proprietary examples

This allows the development process and technical approach behind Maclyn to be reviewed without publishing proprietary application source code.

---

## About the Developer

I am a business, data, education, and nonprofit professional transitioning back into hands-on analytics and technology.

My background includes SQL reporting, Microsoft Excel, quality assurance, business analysis, Informatica training, staff leadership, education, and nonprofit management.

Maclyn Outdoors is both a product I am developing and a practical demonstration of my current work with data, application development, APIs, testing, problem-solving, and technology.

**GitHub:** MikeWalterII

**Project:** Maclyn Outdoors — Outdoor Intelligence

**Tagline:** Know. Decide. Go.
