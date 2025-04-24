# Android Lab Exercise: Task Manager Application

## Overview

In this lab, you will build a Task Manager Android application that allows users to create, view, edit, and delete tasks. This project will help you practice fundamental Android development concepts including RecyclerView, custom dialogs, menu customization, and UI styling.

## Learning Objectives

- Implement a RecyclerView with custom adapter
- Create and style AlertDialogs
- Customize menu items appearance
- Apply themes and styles
- Handle user interactions and data management

## Requirements

### Main Activity Features

- **RecyclerView** to display a list of tasks
- **Floating Action Button** to add new tasks
- **Toolbar** with custom menu items:
  - Search
  - Add task
  - Refresh
  - Settings

### Task Item Components

Each task should include:
- Title (required)
- Description (optional)
- Priority level (High, Medium, Low)
- Due date
- Completion status

### User Interactions

- **Tap on task**: Toggle completion status
- **Long press on task**: Open edit dialog
- **FAB press**: Open add task dialog
- **Menu interactions**: Implement appropriate actions

### UI Customization Requirements

- Create a custom color scheme
- Style AlertDialog buttons with custom colors and text appearance
- Apply custom styling to menu items
- Add visual indicators for task priority levels

## Implementation Steps

### Step 1: Project Setup

1. Create a new Android project with an Empty Activity
2. Set up the basic project structure
3. Define colors and styles in the appropriate resource files
4. Add necessary dependencies in the build.gradle file

### Step 2: Data Mode

Create a Task class with the following properties:
- ID (int)
- Title (String)
- Description (String)
- Priority (enum or int)
- Due date (String or Date)
- Completion status (boolean)

Include appropriate constructors, getters, and setters.

### Step 3: Layout Resources

Create the following layout resources:
1. **Main Activity Layout** with:
   - Toolbar
   - RecyclerView
   - Floating Action Button

2. **Task Item Layout** with:
   - Priority indicator (colored bar)
   - Task title and description
   - Due date
   - Checkbox for completion status
   
3. **Task Dialog Layout** for adding/editing tasks:
   - Title input field
   - Description input field
   - Priority selection (radio buttons)
   - Due date selector
   - Save/Cancel buttons

### Step 4: Menu Resources

Create a menu XML file with the following items:
- Search (with icon)
- Add (with icon)
- Refresh (with icon)
- Settings (overflow menu)

### Step 5: Custom Styling

1. Create a custom theme for your application
2. Style AlertDialog buttons:
   - Customize colors for positive, negative, and neutral buttons
   - Change text appearance (size, style, etc.)
3. Style menu items:
   - Apply custom colors to icons and text
   - Customize appearance of overflow menu items

### Step 6: Task Adapter and RecyclerView

1. Create a custom adapter for the RecyclerView
2. Implement view holder pattern
3. Handle item click events and long presses
4. Display task items with appropriate visual styling based on priority and completion status

### Step 7: Dialog Management

1. Create methods to show add/edit task dialogs
2. Implement dialog button listeners
3. Apply custom styling to dialog buttons
4. Validate user input before saving tasks
