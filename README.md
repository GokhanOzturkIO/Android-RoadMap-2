# Android-RoadMap-2 `v1.0.0-alpha01`

**Androidv14 - Level34**

## UI GUIDE

### 1. Develop your app’s layout

#### 1.1 About layouts
- Layouts in Views
- Write the XML
- Load the XML resource
- Attributes
    - ID
    - Layout parameters
- Layout position
- Size, padding, and margins
- Common layouts
- Build dynamic lists
    - Fill an adapter view with data
    - Handle click events
 
#### 1.2 Responsive/adaptive design with views
- Responsive design
    - ConstraintLayout
    - Responsive width and height
- Adaptive design
    - SlidingPaneLayout for list-detail UIs
    - Alternative layout resources
    - Window size classes
    - Modularized UI components using fragments
    - Activity embedding
- Screen sizes and aspect ratios

#### 1.3 Build a responsive UI with ConstraintLayout
- Constraints overview
- Add ConstraintLayout to your project
    - Convert a layout
    - Create a new layout
- Add or remove a constraint
    - Parent position
    - Order position
    - Alignment
    - Baseline alignment
    - Constrain to a guideline
    - Constrain to a barrier
- Adjust the constraint bias
- Adjust the view size
    - Set size as a ratio
- Adjust the view margins
- Control linear groups with a chain
- Automatically create constraints
- Keyframe animations

#### 1.4 Create dynamic lists with RecyclerView
- Key classes
- Steps for implementing your RecyclerView
- Plan your layout
- Implement your adapter and view holder

#### 1.5 Customize a dynamic list
- Modify the layout
- Add item animations
- Enable list-item selection

#### 1.6 Create a card-based layout
- Add the dependencies

#### 1.7 Create a two pane layout
- Setup
- XML layout configuration
- Programmatically swap out the detail pane
- Navigation component implementation
- Integrate with the system back button
- Lock mode

#### 1.8 Create a linear layout
- Layout weight
    - Equal distribution
    - Unequal distribution

#### 1.9 AdapterView
- Fill the layout with data
- Handle user selections

#### 1.10 Relative Layout
- Positioning Views

#### 1.11 Improve layout performance

##### 1.11.1 About layout performance
- Lessons

##### 1.11.2 Optimize layout hierarchies
- Inspect your layout
- Revise your layout
- Use lint

##### 1.11.3 Reuse layouts with `<include>`
- Create a reusable layout
- Use the `<include>` tag
- Use the `<merge>` tag

##### 1.11.4 Load views on demand
- Define a ViewStub
- Load the ViewStub layout

#### 1.12 Create custom view components

##### 1.12.1 About custom view components
- The basic approach
- Fully customized components
    - Extend onDraw() and onMeasure()
- Compound controls
- Modify an existing view type

##### 1.12.2 How Android draws Views
- Initiate a measure pass
- Initiate a layout pass
- Implement a custom measurement and layout logic

##### 1.12.3 Create a view class
- Subclass a view
- Define custom attributes
- Apply custom attributes
- Add properties and events
- Design for accessibility

##### 1.12.4 Create a custom drawing
- Override onDraw()
- Create drawing objects
- Handle layout events
- Draw
- Apply graphics effects

##### 1.12.5 Make a custom view interactive
- Handle input gestures
- Create physically plausible motion
- Make your transitions smooth

##### 1.12.6 Optimize a custom view
- Speed up your view

#### 1.13 Work with window insets and cutouts

##### 1.13.1 Lay out your app within window insets

##### 1.13.2 Display content edge-to-edge in your app
- Enable the edge-to-edge display
- Handle overlaps using insets
    - System bars insets
    - System gesture insets
- Immersive mode

##### 1.13.3 Insets: Apply rounded corners
- Be careful of clipping

##### 1.13.4 Hide system bars for immersive mode

##### 1.13.5 Support display cutouts
- Choose how your app handles cutout areas
    - Default behavior
    - Render content in short edge cutout areas
    - Never render content in the display cutout area
- Best practices for display cutout support
- Test how your content renders

##### 1.13.6 Control and animate the software keyboard
- Prerequisites
- Check keyboard software visibility
- Synchronize animation with the software keyboard

#### 1.14 Add web-based content to your app

##### 1.14.1 About web-based content
- Alternatives to WebView

##### 1.14.2 Build web apps in WebView
- Work with WebView on earlier versions of Android
- Add a WebView to your app
    - Add a WebView in the activity layout
    - Add a WebView in onCreate()
- Use JavaScript in WebView
    - Enable JavaScript
    - Bind JavaScript code to Android code
- Handle page navigation
    - Handle custom URLs
    - Navigate web page history
    - Handle device configuration changes
- Manage windows

##### 1.14.3 Manage WebView objects
- Version API
- Google Safe Browsing Service
    - Define programmatic actions
- HTML5 Geolocation API
- Opt out of metrics collection
- Termination Handling API
- Renderer Importance API

##### 1.14.4 Load in-app content
- WebViewAssetLoader
    - Create in-app assets and resources
    - Mix in-app content with resources from your website
- loadDataWithBaseURL
- Things to avoid

##### 1.14.5 Darken web content in WebView
- Content-author styling
- Algorithmic darkening
    - Allow algorithmic darkening for web content with Force Dark
    - Allow algorithmic darkening (apps targeting Android 13 or higher)
    - Allow algorithmic darkening (apps targeting Android 12 or lower)

##### 1.14.6 Support different screens in web apps
- Specify viewport properties
- Target device density with CSS
- Target device density with JavaScript

##### 1.14.7 Debug web apps
- Use console APIs in WebView
- Test experimental web features

##### 1.14.8 Best practices for web apps

##### 1.14.9 User privacy in WebView reporting
- Usage statistics
    - Opt out usage statistics
    - Opt out of metrics collection
- Crash reports
- Pseudonymous identifiers and data privacy

##### 1.14.10 Beta program
- How do I subscribe to the Beta program?
- How do I unsubscribe from the Beta program?
- Other ways to test WebView
- Webview DevTools
    - Webview Crashes
    - Webview Flags
- Using WebView on older versions of Android

##### 1.14.11 Beta program
- JavaScript Evaluation
- Basic Usage
- Handling Sandbox Crashes
- Optional Sandbox Features
- Passing Parameters
- Running Wasm Code
- JavaScriptIsolate Separation
- Kotlin Support
- Configuration Parameters

---

### **2. Apply themes**

#### 2.1 Styles and themes

- **Themes versus styles**
- **Create and apply a style**
- **Extend and customize a style**
- **Apply a style as a theme**
- **Style hierarchy**
    - **TextAppearance**
- **Customize the default theme**
    - **Add version-specific styles**
- **Customize widget styles**

#### 2.2 Enable users to personalize their color experience in your app

- How Android creates color schemes
- How color variants display on a user's device
- Get started with Compose
- Get started with Views
    - Create your theme with tokens
    - Retain custom or brand colors
- Apply Dynamic Color to your adaptive icons and widgets

#### 2.3 Select colors with the Palette API

- Set up the library
- Create a palette
    - Generate a Palette instance
    - Customize your palette
- Extract color profiles
    - Use swatches to create color schemes

#### 2.4 Material Design for Android

- Material theme and widgets
- Elevation shadows and cards
- Animations
- Drawables

#### 2.5 Implement dark theme

- Support dark theme in your app
    - Themes and styles
    - Change themes in-app
- Force Dark
    - Disable Force Dark on a view
- Web content
- Best practices
    - Notifications and widgets
    - Launch screens
    - Configuration changes

#### 2.6 Create shadows and clip views

- Assign elevation to your views
- Customize view shadows and outlines
- Clip views

---

#### 3. Add components

#### 3.1 Add core components

##### 3.1.1 Add a floating action button

- Add the floating action button to your layout
- Respond to button taps

##### 3.1.2 Add buttons to your app

- Respond to click events
- Style your button
    - Borderless button
    - Custom background

##### 3.1.3 Add checkboxes to your app

- Respond to click events

##### 3.1.4 Add radio buttons to your app

- Respond to click events

##### 3.1.5 Add toggle buttons

- Handle state changes

##### 3.1.6 Add pickers to your app

- Create a time picker
    - Extend DialogFragment for a time picker
    - Show the time picker
- Create a date picker
    - Extend DialogFragment for a date picker
    - Show the date picker
- Use pickers with autofill

##### 3.1.7 Tooltips

- Setting the tooltip text

##### 3.1.8 Dialogs

- Create a dialog fragment
- Build an alert dialog
    - Add buttons
    - Add a list
    - Create a custom layout
- Pass events back to the dialog's host
- Show a dialog
- Show a dialog fullscreen or as an embedded fragment
    - Show an activity as a dialog on large screens
- Dismiss a dialog

##### 3.1.9 Add menus

- Define a menu in XML
- Create an options menu
    - Handle click events
    - Change menu items at runtime
- Create a contextual menu
    - Create a floating context menu
    - Use the contextual action mode
- Create a popup menu
    - Handle click events
- Create a menu group
    - Use checkable menu items
- Add menu items based on an intent
    - Let your activity be added to other menus

#### 3.2 Add the app bar component

##### 3.2.1 Add the app bar

##### 3.2.2 Set up the app bar

- Add a Toolbar to an Activity
- Use app bar utility methods

##### 3.2.3 Add and handle actions

- Add action buttons
- Respond to actions

##### 3.2.4 Add an Up action

- Configure your app bar

##### 3.2.5 Use action views and action providers

- Add an action view
    - Respond to action view expansion
- Add an action provider
- Additional resources

#### 3.3 Add the settings component

##### 3.3.1 Settings

- Get started
    - Create a hierarchy
    - Inflate the hierarchy
- Monitor the preferences
- Read the current preference value

##### 3.3.2 Organize your settings

- Preference categories
- Split your hierarchy into multiple screens
    - PreferenceScreens
    - Use separate Activities

##### 3.3.3 Customize your settings

- Find preferences
- Control Preference visibility
- Dynamically update summaries
    - Use a SimpleSummaryProvider
    - Use a custom SummaryProvider
- Customize an EditTextPreference dialog
- Preference actions
    - Set an Intent
    - OnPreferenceClickListener

##### 3.3.4 Use saved Preference values

- Preference data storage
    - SharedPreferences
    - PreferenceDataStore
- Read Preference values
- Listen for changes to Preference values
    - Implement OnPreferenceChangeListener
    - Implement OnSharedPreferenceChangeListener
- Use a custom datastore
    - Implement the datastore
    - Enable the datastore

##### 3.3.5 Create a hierarchy in code

##### 3.3.6 Handle other form factors

- Android TV

##### 3.3.7 Preference components and attributes

- Preference components
    - Preference infrastructure
    - Preference containers
    - Individual Preferences
- Preference attributes
    - Generic attributes
    - PreferenceCategory attributes
    - ListPreference / MultiSelectListPreference attributes

##### 3.3.8 Integrate Android search component

###### **3.3.8.1 Integrate Android search features into your app**

- Protect user privacy

###### **3.3.8.2 Create a search interface**

- The basics
- Create a searchable configuration
- Create a searchable activity
    - Declare a searchable activity
    - Perform a search
- Use the search dialog
    - Invoke the search dialog
    - The impact of the search dialog on your activity lifecycle
    - Pass search context data
- Use the search widget
    - Configure the search widget
    - Other search widget features
    - Use both the widget and the dialog
- Add voice search
- Custom search suggestions

###### **3.3.8.3 Add custom search suggestions**

- The basics
- Create a content provider
- Modify the searchable configuration
- Save queries
- Clear the suggestion data

###### **3.3.8.4 Add custom search suggestions**

- The basics
- Modify the searchable configuration
- Create a content provider
    - Handle the suggestion query
    - Build a suggestion table
- Declare an intent for suggestions
    - Declare the intent action
    - Declare intent data
- Handle the intent
- Rewrite the query text
- Expose search suggestions to Quick Search Box
    - Enable suggestions on a device
    - Manage Quick Search Box suggestion shortcuts
    - About Quick Search Box suggestion ranking

###### **3.3.8.5 Search configuration**

###### **3.3.8.6 AppSearch**

- Setup
- AppSearch concepts
    - Database and session
    - Schema and schema types
    - Documents
    - Search
- Platform Storage vs Local Storage
- Get started with AppSearch
    - Write a document class
    - Open a database
    - Set a schema
    - Put a document in the database
    - Search
    - Iterate through SearchResults
    - Remove a document
    - Persist to disk
    - Close a session

###### **3.3.8.7 Add search functioality**

###### **3.3.8.7.1 Add search functionality**

###### **3.3.8.7.2 Set up the search interface**

- Add the SearchView to the app bar
- Create a search configuration
- Create a searchable activity

###### **3.3.8.7.3 Storing and Searching for Data**

- Create the Virtual Table
- Populate the Virtual Table
- Search for the Query

###### **3.3.8.7.4 Remaining Backward Compatible**

- Set Minimum and Target API levels
- Provide the Search Dialog for Older Devices
- Check the Android Build Version at Runtime
