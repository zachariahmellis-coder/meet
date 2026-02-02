# Meet App — CareerFoundry Achievement 4 (Exercise 4.1)

## Overview

Meet is a serverless progressive web application (PWA) built with React. The app allows users to discover upcoming events for a selected city, view and manage event details, control how many events are displayed, use the app while offline, add a shortcut to the home screen, and visualize event data using charts.

The project is designed with slow-travel use cases in mind—such as planning events while moving between cities during a trip (e.g., a long-term stay in Japan)—where reliable access, offline support, and quick scanning of information are essential.

This exercise focuses on defining user stories and test scenarios using a test-driven and behavior-driven development (TDD/BDD) approach.

---

## Tech Stack

- React (Vite)
- JavaScript
- GitHub
- Vercel
- AWS (account created for upcoming serverless exercises)

---

## Features, User Stories, and Scenarios

### Feature 1: Filter Events by City

**User Story**  
As a user traveling between cities, I should be able to filter events by city, so that I can see what’s happening in the place I’m currently staying.

**Scenarios**

- **Given** the user hasn’t searched for a city,  
  **When** the user opens the app,  
  **Then** a list of upcoming events from all cities is shown.

- **Given** the main page is open,  
  **When** the user starts typing in the city search box,  
  **Then** a list of matching city suggestions is displayed.

- **Given** city suggestions are displayed,  
  **When** the user selects a city from the list,  
  **Then** upcoming events for that city are shown.

---

### Feature 2: Show / Hide Event Details

**User Story**  
As a user, I should be able to show or hide event details, so that I can quickly scan events and expand only the ones I’m interested in.

**Scenarios**

- **Given** events are displayed,  
  **When** the user views the event list,  
  **Then** event details are collapsed by default.

- **Given** event details are collapsed,  
  **When** the user clicks the “Show details” button,  
  **Then** the event details are expanded.

- **Given** event details are expanded,  
  **When** the user clicks the “Hide details” button,  
  **Then** the event details are collapsed.

---

### Feature 3: Specify Number of Events

**User Story**  
As a user, I should be able to specify the number of events displayed, so that I can avoid information overload while planning my days.

**Scenarios**

- **Given** the app is opened,  
  **When** the event list is displayed,  
  **Then** a default number of events is shown.

- **Given** the event list is displayed,  
  **When** the user changes the number of events,  
  **Then** the event list updates to reflect that number.

---

### Feature 4: Use the App When Offline

**User Story**  
As a user traveling with limited or unreliable connectivity, I should be able to use the app when offline, so that I can still access event information on the go.

**Scenarios**

- **Given** the app has been used while online,  
  **When** the user opens the app offline,  
  **Then** cached event data is displayed.

- **Given** the user is offline,  
  **When** the user attempts to change the city or refresh data,  
  **Then** an error or warning message is shown.

---

### Feature 5: Add an App Shortcut to the Home Screen

**User Story**  
As a user, I should be able to add the app shortcut to my home screen, so that I can quickly access it like a native travel app.

**Note**  
This feature is handled by the browser or operating system and is not directly tested within the app.

---

### Feature 6: Display Charts Visualizing Event Details

**User Story**  
As a user, I should be able to view charts visualizing event details, so that I can better understand event distribution across cities.

**Scenarios**

- **Given** event data is available,  
  **When** the user views the app,  
  **Then** charts visualizing event data are displayed.

- **Given** charts are displayed,  
  **When** the user changes the city filter,  
  **Then** the charts update to reflect the new data.

---

## Deployment

This project is deployed using Vercel. Each push to the main branch triggers an automatic redeployment.

## Links

GitHub Repository: (add link)
Live App (Vercel): (add link)

## AWS

An AWS account was created as part of Exercise 4.1 in preparation for upcoming serverless function development.

## Setup

```bash
npm install
npm run dev
```
