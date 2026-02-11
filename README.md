# Dashboard & Visualization Management

## Overview
This repository demonstrates how a ServiceNow dashboard and data visualization were created to monitor the Infinity HHD service offering. The implementation focused on building a centralized dashboard, generating dynamic visualizations from incident data, and sharing access with appropriate support groups.

This project simulates a real-world scenario where a product owner requires visibility into service performance and incident trends through interactive analytics.

## Use Case
As organizations scale their service offerings, stakeholders need a single source of truth to monitor incidents and identify patterns such as pilot participation, inquiry volume, and firmware-related issues.

In this scenario, the Infinity HHD product owner required a dashboard that displayed incident data with flexible grouping options. The dashboard needed to support dynamic filtering while remaining accessible to the Training Technology Support team for ongoing monitoring and collaboration.

This project reflects a practical implementation of ServiceNow Platform Analytics for operational visibility.

## Features
- Custom dashboard creation using inline editor
- Dynamic data visualization from incident lists
- Donut chart visualization with multiple grouping dimensions
- Interactive group-by selector for real-time analysis
- Bookmarking and reuse of saved visualizations
- Dashboard sharing with role-based edit permissions

## Technologies Used
- ServiceNow Platform
- Platform Analytics
- Dashboards
- Data Visualizations
- Incident Management
- Role and Group Access Control

## Implementation Walkthrough

### Objective
Create a dashboard for monitoring the Infinity HHD service offering, build a dynamic incident visualization, and share dashboard access with the appropriate support group.

### Step 1: Create the Infinity HHD Product Monitoring Dashboard
The dashboard interface was accessed as a System Administrator to ensure full configuration permissions.

A new dashboard named **Infinity HHD Product Monitoring** was created using the inline editor to support drag-and-drop visualization management.

The dashboard was saved and confirmed to load successfully as an empty canvas, ready for data elements.

### Step 2: Prepare Incident Test Data for Visualization
Incident records associated with the Infinity HHD service offering were reviewed to ensure sufficient data variety.

Additional incidents were created to represent:
- Inquiry incidents marked as Pilot
- Hardware incidents with Firmware subcategory
- Hardware incidents not marked as Pilot

This ensured the dataset supported multiple grouping dimensions required for analysis.

<img width="1901" height="210" alt="Screen Shot 2026-02-10 at 8 12 53 PM" src="https://github.com/user-attachments/assets/43827433-3d51-42e6-b693-d2a96c9fe873" />

### Step 3: Create a Visualization from the Incident List
The Infinity HHD incident list was filtered and reviewed to confirm correct service offering context.

A visualization was launched directly from the **Pilot** column using the list column options menu, creating a pie-based report in the Visualization Designer.

The visualization type was updated to a **Donut** chart to improve readability and distribution clarity.

### Step 4: Configure Dynamic Grouping Options
The visualization details were updated and renamed to **HHD Incidents – by Pilot, Inquiry, Firmware**.

An alternative group-by selector was enabled and configured to allow switching between:
- Pilot
- Category
- Subcategory

The selector was set to be visible by default, allowing users to dynamically change perspectives without modifying the report configuration.

<img width="1901" height="820" alt="Screen Shot 2026-02-10 at 8 24 28 PM" src="https://github.com/user-attachments/assets/3b7e3e6b-9666-48a9-ac26-ee868483d685" />


### Step 5: Save and Validate the Visualization
The visualization was saved and validated to confirm:
- Correct incident counts
- Accurate Pilot true vs false distribution
- Functional group-by selector behavior

Selecting individual segments of the donut chart successfully filtered the underlying incident list, confirming interactive functionality.

<img width="1901" height="858" alt="Screen Shot 2026-02-10 at 8 26 08 PM" src="https://github.com/user-attachments/assets/4ef5e1be-d387-468b-89b5-6be24fa1a7a4" />

### Step 6: Add the Visualization to the Dashboard
The saved visualization was located within the Platform Analytics library and added to the **Infinity HHD Product Monitoring** dashboard.

The visualization was resized and positioned on the dashboard canvas to optimize visibility.

Dashboard changes were saved to preserve layout and configuration.

<img width="1901" height="319" alt="Screen Shot 2026-02-10 at 8 30 33 PM" src="https://github.com/user-attachments/assets/f62a63e8-03f8-414e-b522-b3e241bdb2e0" />

<img width="1901" height="639" alt="Screen Shot 2026-02-10 at 8 33 45 PM" src="https://github.com/user-attachments/assets/36c48dc5-4465-4f7e-af2d-e0701bfb341a" />

<img width="1901" height="729" alt="Screen Shot 2026-02-10 at 8 34 15 PM" src="https://github.com/user-attachments/assets/ed07be5d-8b08-42f3-8b44-38e5aa2648ce" />

### Step 7: Bookmark the Visualization
The visualization was added to bookmarks to support quick access and reuse across dashboards and analytics workflows.

This ensured the visualization could be easily referenced without navigating through the analytics library.

### Step 8: Share Dashboard Access with Support Group
The dashboard sharing options were accessed through the More Actions menu.

Edit-level access was granted to the **Training Technology Support** group, allowing members to add or modify dashboard elements.

Sharing permissions were confirmed to ensure group members could collaborate without requiring administrative access.

<img width="1901" height="729" alt="Screen Shot 2026-02-10 at 8 35 04 PM" src="https://github.com/user-attachments/assets/f2fc66ff-3b8f-4233-8dfa-6d34b5401049" />

## Lessons Learned
- Dashboards provide a centralized view for service offering health
- Dynamic group-by selectors enable flexible, real-time data analysis
- Visualizations created from lists accelerate analytics development
- Donut charts improve clarity for proportional comparisons
- Proper sharing configuration is critical for team collaboration
- Saving and bookmarking visualizations promotes reuse and consistency
