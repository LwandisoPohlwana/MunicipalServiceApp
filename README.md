# MunicipalServiceApp
# Municipal Services Application - README

## Overview
This C# .NET Framework Windows Forms application allows citizens to report problems with municipal services. Users can submit reports with media attachments, including details about the location, category, and description. This guide will help you learn how to run, compile, and utilize the application.

## Environment Guidelines
Before compiling and running the application, ensure you have the following:

1. **Visual Studio**: Install Visual Studio 2019 or later.
   - You can download it from the official [Microsoft Visual Studio website](https://visualstudio.microsoft.com/).
2. **.NET Framework**: Ensure you have the .NET Framework 4.7.2 (or higher) installed.
3. **Operating System**: This application is designed for Windows systems.

## How to Compile the Application

### Open the Project in Visual Studio:
1. Clone or download the project repository.
2. Open Visual Studio and go to **File → Open → Project/Solution**.
3. Navigate to the folder where the project is located and select the `MunicipalServices.sln` solution file.

### Build the Project:
1. Once the project is open, go to the **Build** menu and click on **Build Solution** (or press `Ctrl + Shift + B`).
2. Visual Studio will compile the project. Check the "Output" window to ensure there are no errors.

## How to Run the Application

### Start the Application:
1. After successfully building the solution, you can run the application by clicking the **Start** button in the toolbar.
2. The application should launch, displaying the main menu.

## Using the Application

### Report Issues:
1. From the main menu, choose the **"Report Issues"** option to submit a report.
2. Fill in the location, select a category, and provide a description of the issue.
3. Attach media files (images, documents) to the report by clicking the **"Attach File"** button.
4. Submit the issue by clicking the **"Submit"** button. A success message will appear, and the issue will be saved.

### Local Events and Announcements:
1. From the main menu, select **"Local Events and Announcements"** to view upcoming events and announcements in your area.
2. Use the search bar at the top of the page to find specific events by typing keywords or event names.
3. Use the category filter dropdown to narrow down events based on type (e.g., cultural, sports, community).
4. Events will be displayed in a `DataGridView`, showing key details such as event name, date, and location.
5. Announcements will be displayed in a `ListBox`, with important announcements marked differently.
6. A personalized recommendation section under the search bar will update every few seconds with event suggestions based on your search history and preferences.

### Service Request Status:
1. Access the **Service Request Status** section from the main menu to see a list of all submitted requests.
2. Each request shows details like Request ID, category, priority, and current status.
3. Use the Priority Filter dropdown to sort requests by priority (e.g., high to low urgency).
4. Click **Clear Filter** to reset both filters and view all requests.

## Data Structures Used
To manage and present information across multiple features efficiently, the Municipal Services Application utilizes various data structures:

- **Binary Search Tree (BST)**: Used to organize and retrieve service requests by Request ID in the Service Request Status feature for quick searching.
  
- **Heap**: Used to classify service requests by priority (high to low) in the Service Request Status feature, ensuring high-priority requests are shown first.

- **Queue**: Implemented to control a rolling presentation of customized event suggestions in Local Events and Announcements functionality.

- **Set**: Used to track individual user preferences for event recommendations in Local Events and Announcements, preventing duplicate suggestions.

- **Dictionary**: Used to manage event data and announcements in both Local Events and Announcements and Service Request Status features for fast lookups using unique identifiers.

