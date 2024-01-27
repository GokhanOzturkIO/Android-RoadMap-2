# Android-RoadMap-2 `v1.0.0-alpha01`

**Androidv14 - Level34**

## UI GUIDE - VIEW STRUCTURE

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

---

#### 4. Work with text and emoji

#### 4.1 Autosize TextViews

- Set up TextView autosize
    - Default
    - Granularity
    - Preset sizes

#### 4.2 Use Downloadable Fonts

- How does Downloadable Fonts work?
- The basics
- Use Downloadable Fonts with Android Studio and Google Play services
- Use Downloadable Fonts programmatically
- Use Downloadable Fonts with AndroidX Core
- Use Downloadable Fonts as resources in XML
- Pre-declare fonts in the manifest
- Add certificates

#### 4.3 Add a font as an XML resource

- Create a font family
- Use fonts in XML layouts
- Use fonts programmatically
- Use the Support Library

#### 4.4 Add emoji support

##### 4.4.1 Support modern emoji

- Emoji support in Compose
- Prerequisites
- Use AppCompat to support the latest emoji
    - If your app is using AppCompat but displays tofu (☐)
- Support emoji without AppCompat
    - Use EmojiCompat without widgets
    - Use EmojiCompat for input method editors
- Use emoji in custom views
    - Add custom views for apps with AppCompat
    - Add custom views for apps without AppCompat
- Optional features for handling emoji2
    - Configure emoji2 to use a different font or downloadable font provider
    - Add initialization listeners
    - Support bundled fonts with emoji2
- Impact of automatic EmojiCompat configuration

##### 4.4.2 Add a floating action button

- How does EmojiCompat work?
- Downloadable fonts configuration
    - Adding support library dependency
    - Initializing the downloadable font configuration
- Library components
- Configuration options
- Adding initialization listeners
- Using EmojiCompat with AppCompat widgets
- Bundled fonts configuration
    - Adding support library dependency
    - Using bundled fonts to configure EmojiCompat
- Using EmojiCompat without widgets
- Using EmojiCompat for IMEs
- Using EmojiCompat with custom widgets
- Frequently asked questions

##### 4.4.3 Emoji Picker

- Features
    - Up-to-date Emojis
    - Sticky variants
    - Recent emoji
    - Compatibility with `EmojiCompat`****
- Prerequisites
- Use the library

#### 4.5 Implement a text magnifier

- API usage
- Magnify on user interaction
- Additional considerations when magnifying text

#### 4.6 Spans

- Create and apply a span
- Android span types
    - Spans that affect text appearance
    - Spans that affect text metrics
    - Spans that affect paragraphs
- Create custom spans
- Test span usage
- Test custom spans
- Best practices for using spans
    - Attach or detach a span without changing the underlying text
    - Set text in a TextView multiple times
    - Change internal span attributes
    - Use Android KTX extension functions

---

#### 5. Display graphics and videos

#### 5.1 Static images

##### 5.1.1 Drawables overview

- Create drawables from resource images
- Create drawables from XML resources
- Shape drawables
- NinePatch drawables
- Custom drawables
- Add tint to drawables
- Extract prominent colors from an image

##### 5.1.2 Vector drawables overview

- Key points
- Introduction
- About VectorDrawable class
    - Example XML
- About AnimatedVectorDrawable class
    - Multiple XML files
    - Single XML file
- Vector drawables backward compatibility solution
    - Single XML file

##### 5.1.3 Handling bitmaps

##### 5.1.4 Reducing image download sizes

- About image formats
    - AVIF
    - PNG
    - JPG
    - WebP
- Selecting a format
- Determine optimal quality values
    - Scalar values (JPG and WebP only)
    - Butteraugli
- Serving sizes

##### 5.1.5 Hardware acceleration

- Control hardware acceleration
- Determine if a view is hardware accelerated
- Android drawing models
    - Software-based drawing model
    - Hardware accelerated drawing model
- Support for drawing operations
    - Canvas scaling
- View layers
    - View layers and animations
- Tips and tricks

#### 5.2 Add media playback controls to your app

#### 5.3 Add videos using picture-in-picture (PiP) 

- How users can interact with the PiP window
- Declare PiP support
- Switch your activity to PiP
- Recommended: provide users a polished PiP transition experience
    - Make transitions to PiP mode smoother from gesture navigation
    - Set a proper `sourceRectHint` for entering and exiting PiP mode
    - Disable seamless resizing for non-video content
- Handle UI during PiP
    - Add controls
- Continuing video playback while in PiP
- Use a single playback activity for PiP
- Best practices

#### 5.4 Work with advanced images and graphics

##### 5.4.1 Draw with AGSL shaders

###### **5.4.1.1 Android Graphics Shading Language (AGSL)**

- Theory of operation
- Basic syntax

###### **5.4.1.2 Differences between AGSL and GLSL**

- Shader execution
- Coordinate space
- Precision and types
- Preprocessor
- Color spaces
    - Uniforms

###### **5.4.1.3 Using AGSL in your Android app**

- A simple AGSL shader
- Drawing the gradient
- Animating the shader
- Painting complex objects
- Shading and Canvas transformations
- Using RuntimeShader with Jetpack Compose
- Using RuntimeShader with RenderEffect

###### **5.4.1.4 AGSL Quick Reference**

- Types
    - Basic types
    - Precision and range minimums
    - Structures and arrays
- Qualifiers
- Variable declaration
- Matrix/structure/array basics
    - Matrix constructor examples
    - Structure constructor example
    - Matrix components
    - Structure fields
    - Array elements
- Operators
    - Matrix and vector operations
- Program control
    - For loop limitations
- Built-in functions
    - Angle & trigonometric functions
    - Exponential functions
    - Common functions
    - Geometric functions
    - Matrix functions
    - Vector relational functions
    - Color functions
- Shader sampling (evaluation)
- Raw buffer sampling

##### 5.4.2 Use OpenGL ES for graphics

###### **5.4.2.1 OpenGL ES**

- The basics
    - OpenGL ES packages
- Declaring OpenGL requirements
- Mapping coordinates for drawn objects
    - Projection and camera view in OpenGL ES 1.0
    - Projection and camera view in OpenGL ES 2.0 and higher
- Shape faces and winding
- OpenGL versions and device compatibility
    - Texture compression support
    - Determining OpenGL extensions
    - Checking the OpenGL ES version
- Choosing an OpenGL API version

###### **5.4.2.2 Learn how to use Open GL ES with graphics**

###### **5.4.2.2.1 Displaying graphics with OpenGL ES**

- Lessons

###### **5.4.2.2.2 Build an OpenGL ES environment**

- Declare OpenGL ES use in the manifest
- Create an activity for OpenGL ES graphics
- Build a GLSurfaceView object
- Build a renderer class

###### **5.4.2.2.3 Define shapes**

- Define a triangle
- Define a square

###### **5.4.2.2.4 # **Draw shapes**

- Initialize shapes
- Draw a shape

###### **5.4.2.2.5 Apply projection and camera views**

- Define a projection
- Define a camera view
- Apply projection and camera transformations

###### **5.4.2.2.6 Add motion**

- Rotate a shape
- Enable continuous rendering

###### **5.4.2.2.7 Respond to touch events**

- Setup a touch listener
- Expose the rotation angle
- Apply rotation

###### **5.4.2.2.8 Creating multiple APKs for different GL textures**

- Confirm you need multiple APKs
- Chart your requirements
- Put all common code and resources in a library project
- Create new APK projects
- Adjust the manifests
- Review your pre-launch checklist

---

#### 6. Work with animations and transitions

#### 6.1 Static images

- Documentation
- Videos

#### 6.2 Introduction to animations

- Animate bitmaps
- Animate UI visibility and motion
    - Physics-based motion
- Animate layout changes
- Animate between activities

#### 6.3 Property Animation Overview

- How property animation works
- How property animation differs from view animation
- API overview
- Animate using ValueAnimator
- Animate using ObjectAnimator
- Choreograph multiple animations using an AnimatorSet
- Animation listeners
- Animate layout changes to ViewGroup objects
- Animate view state changes using StateListAnimator
- Use a TypeEvaluator
- Use Interpolators
- Specify keyframes
- Animate views
    - Animate using ViewPropertyAnimator
- Declare animations in XML
- Potential effects on UI performance

#### 6.4 Animate drawable graphics

- Use AnimationDrawable
- Use AnimatedVectorDrawable
    - Animated Vector Drawable (AVD) preview

#### 6.5 Animate views

##### 6.5.1 View Animation

##### 6.5.2 Reveal or hide a view using animation

- Create a crossfade animation
    - Create the views
    - Set up the crossfade animation
    - Crossfade the views
- Create a card flip animation
    - Create the animator objects
    - Create the views
    - Create the fragments
    - Animate the card flip
- Create a circular reveal animation

##### 6.5.3 Move a View with animation

- Change the view position with ObjectAnimator
- Add curved motion
    - Define your own path
    - Use PathInterpolator

##### 6.5.4 Move views using a fling animation

- Add the AndroidX library
- Create a fling animation
- Set velocity
    - Set an animation value range
    - Set friction
    - Set the minimum visible change

##### 6.5.5 Enlarge a view using a zoom animation

- Create the views
- Set up the zoom animation
- Zoom the view

#### 6.6 Animate movement using spring physics

- Lifecycle of a spring animation
- Build a spring animation
- Add the support library
    - Create a spring animation
    - Register listeners
    - Remove listeners
    - Set animation start value
    - Set animation value range
    - Set start velocity
    - Set spring properties
    - Create a custom spring force
    - Start animation
    - Cancel animation

#### 6.7 Auto-animate layout updates

- Create the layout
- Add, update, or remove items from the layout

#### 6.8 Animate layout changes using a transition

- Create a scene
    - Create a scene from a layout resource
    - Create a scene in your code
    - Create scene actions
- Apply a transition
    - Create a transition
    - Apply a transition
    - Choose specific target views
    - Specify multiple transitions
    - Apply a transition without scenes
    - Define transition lifecycle callbacks
- Limitations

#### 6.9 Create a custom transition animation

- Extend the Transition class
- Capture view property values
    - Capture starting values
    - Capture ending values
- Create a custom animator
- Apply a custom transition

#### 6.10 Start an activity using an animation

- Check the system version
- Specify custom transitions
- Start an activity using transitions
- Start an activity with a shared element
- Start an activity with multiple shared elements

#### 6.11 MotionLayout

##### 6.11.1 Manage motion and widget animation with MotionLayout

- Design considerations
- Get started
- Interpolated attributes
- Custom attributes
    - Change background color
- Additional MotionLayout attributes

##### 6.11.2 Carousel with MotionLayout

- How Carousel with MotionLayout works
    - Transitions
    - Add the Carousel
    - Additional notes

##### 6.11.3 MotionLayout examples

- Basic motion
- Custom attribute - backgroundColor
- ImageFilterView - image transition
- Keyframe position
- Keyframe interpolation
- Keyframe cycle
- CoordinatorLayout (1/2)
- CoordinatorLayout (2/2)
- DrawerLayout (1/2)
- DrawerLayout (2/2)
- Side panel
- Parallax
- ViewPager
- ViewPager - Lottie
- Complex motion (1/3)
- Complex motion (2/3)
- Complex motion (3/3)
- Fragment transition (1/2)
- Fragment transition (2/2)
- YouTube-like motion
- KeyTrigger
- Multi-state

#### 6.12 Slide between fragments

##### 6.12.1 Slide between fragments using ViewPager2

- Create the views
- Create the fragment
- Add a ViewPager2
- Customize the animation using PageTransformer
    - Zoom-out page transformer
    - Depth page transformer
- Additional resources

##### 6.12.2 Slide between fragments using ViewPager

- Create the views
- Create the fragment
- Add a ViewPager
- Customize the animation using PageTransformer
    - Zoom-out page transformer
    - Depth page transformer

##### 6.12.3 Migrate from ViewPager to ViewPager2

- Benefits of migrating to ViewPager2
    - Vertical orientation support
    - Right-to-left support
    - Modifiable fragment collections
    - DiffUtil
- Migrate your app to ViewPager2
    - Update XML layout files
    - Update adapter classes
    - Refactor TabLayout interfaces
    - Support nested scrollable elements

#### 6.13 Additional resources for animation

- Videos
- Samples

---

#### 7. Receive rich content

---

#### 8. Add support for touch and input

#### 8.1 Touch and input overview

#### 8.2 Input events overview

- Event listeners
- Event handlers
- Touch mode
- Handling focus

#### 8.3 Use touch gestures

##### 8.3.1 About gestures

##### 8.3.2 Detect common gestures

- Gather data
    - Capture touch events for an Activity or View
    - Capture touch events for a single view
- Detect gestures
    - Detect all supported gestures
    - Detect a subset of supported gestures

##### 8.3.3 Track touch and pointer movements

- Track velocity
- Use pointer capture
    - Request pointer capture
    - Handle captured pointer events
    - Release pointer capture
 
##### 8.3.4 Animate a scroll gesture

- Understand scrolling terminology
- Components that contain built-in scrolling implementations
- Create a custom touch-based scrolling implementation
- Implement the stretch overscroll effect
    - Catch the animation
    - Release the overscroll effect
    - Opt out of overscroll

##### 8.3.5 Ensure compatibility with gesture navigation

- Provide edge-to-edge app content
- Handle conflicting app gestures
    - Conflicts with back gestures
    - Conflicts with home or quick-switch gestures
    - Games and other non-View apps
- Update your app to support the predictive back gesture

##### 8.3.6 Handle multi-touch gestures

- Track multiple pointers
    - Start and end gestures
    - Keep track of pointers
- Retrieve `MotionEvent` actions

##### 8.3.7 Drag and scale

- Drag an object
- Drag to pan
- Use touch to perform scaling
    - Basic scaling example
    - More complex scaling example

##### 8.3.8 Manage touch events in a ViewGroup

- Intercept touch events in a ViewGroup
    - Process ACTION_OUTSIDE events
- Use ViewConfiguration constants
- Extend a child view's touchable area

##### 8.3.9 Add support for swipe-to-refresh

###### **8.3.9.1 About swipe-to-refresh**

###### **8.3.9.2 Add swipe-to-refresh to your app**

- Add SwipeRefreshLayout dependency
- Add the SwipeRefreshLayout Widget
- Add a refresh action to the action bar

###### **8.3.9.3 Respond to a refresh request**

- Respond to the refresh gesture
- Respond to the refresh action

#### 8.4 Handle keyboard input

##### 8.4.1 Handle keyboard input

##### 8.4.2 Specify the input method type

- Specify the keyboard type
- Enable spelling suggestions and other behaviors
- Specify the input method action
- Provide auto-complete suggestions

##### 8.4.3 Handle input method visibility

- Show the soft keyboard when the activity starts
    - Specify how your UI should respond
- Show the soft keyboard on demand
    - Show the soft keyboard reliably
    - Handle runtime visibility flags carefully
- System usually hides the soft keyboard automatically
    - Hide the soft keyboard manually based on previous system behavior
- Show a dialog or overlay view on top of the soft keyboard
    - Create a dialog
    - Create an overlay view
- Show a dialog or view underneath the soft keyboard
    - Create a dialog
    - Create an overlay view

##### 8.4.4 Support keyboard navigation

- Test your app
- Handle tab navigation
- Handle directional navigation

##### 8.4.5 Handle keyboard actions

- Handle single key events
- Handle modifier keys

#### 8.5 Stylus

- Detecting stylus input
- Set your experience apart with advanced libraries
- Low latency libraries
- Advanced libraries
- Build for all types of input

#### 8.6 Copy and paste

- The clipboard framework
- Clipboard classes
    - ClipboardManager
    - ClipData, ClipData.Item, and ClipDescription
    - ClipData convenience methods
    - Coerce the clipboard data to text
- Copy to the clipboard
    - Provide feedback when copying to the clipboard
    - Avoid duplicate notifications
    - Add sensitive content to the clipboard
- Paste from the clipboard
    - Paste plain text
    - Paste data from a content URI
    - Paste an Intent
- System notification shown when your app accesses clipboard data
- Use content providers to copy complex data
    - Encode an identifier on the URI
    - Copy data structures
    - Copy data streams
- Design effective copy and paste functionality

#### 8.7 Enable drag and drop

- Overview
    - Drag event listeners and callback methods
    - Drag and drop process
    - Drag events
    - Drag shadow
- A drag and drop operation
    - Start a drag
    - Respond to a drag start
    - Handle events during the drag
    - Respond to a drop
    - Respond to a drag end
    - Respond to drag events: An example
- Drag and drop in multi-window mode
    - Source drag and drop activity
    - Target drag and drop activity
- DropHelper for simplified drag and drop
    - Specify drop targets
    - Configure drop targets
    - Handle data in drop targets
    - MIME types, permissions, and content validation

#### 8.8 Receive rich content

- Overview
- Implementation
- URI permissions
- Custom views
- Comparison with the keyboard image API

#### 8.9 Implement tactile feedback (haptics)

##### 8.9.1 Implement haptics on Android

##### 8.9.2 Haptics design principles

- Use cases for adding haptics to your app
- Haptics classifications
    - Clear haptics
    - Rich haptics
    - Buzzy haptics
- Haptics design guidelines
    - Prioritize predefined haptic constants and effects
    - Correlate event importance and frequency with strength
    - Be consistent
    - Design visual and audio experience together with haptics
    - Avoid legacy one-shot vibrations for haptic feedback

##### 8.9.3 Add haptic feedback to events

- Use `View` components to generate haptic feedback
    - Prerequisites: Enable haptic feedback
    - Choose a `HapticFeedbackConstant`****
    - Example 1: Keypress
    - Example 2: Submit button
- Use a predefined `VibrationEffect` to generate haptic feedback
    - Understand device support of `VibrationEffect` APIs
    - Prerequisites: Load the Vibrator and the `VIBRATE` permission
    - Play a predefined `VibrationEffect`****
- Use advanced compositions with primitives

##### 8.9.4 Vibration actuators primer

##### 8.9.5 Create custom haptic effects

- Use fallbacks to handle device compatibility
- Usage of haptic primitives
- Create custom vibration patterns
    - Sample: Ramp-up pattern
    - Sample: Repeating pattern
    - Sample: Pattern with fallback
- Create vibration compositions
    - Sample: Resist (with low ticks)
    - Sample: Expand (with rise and fall)
    - Sample: Wobble (with spins)
    - Sample: Bounce (with thuds)

##### 8.9.6 Android haptics API reference

- `HapticFeedbackConstants`
    - Compatibility and requirements
    - Usage of `HapticsFeedbackConstants`****
- Predefined `VibrationEffect`****
    - Compatibility and requirements
    - Usage of predefined `VibrationEffect`****
- `VibrationEffect` composition
    - Compatibility and requirements
    - Usage of `VibrationEffect` Compositions
- On-off, one-shot, and waveform vibrations
    - Compatibility and requirements
    - Usage of on-off vibrations
- Notification APIs
- General concepts
    - Does the device have a vibrator?
    - Has the user disabled touch haptics?
    - Vibration attributes
    - Amplitude control

#### 8.10 Add support for game controllers

##### 8.10.1 Support game controllers

##### 8.10.2 Handle controller actions

- Verify a game controller is connected
- Process gamepad button presses
- Process directional pad input
- Process joystick movements

##### 8.10.3 Support controllers across android versions

- Prepare to abstract APIs for game controller support
- Add an interface for backward compatibility
- Implement the interface on Android 4.1 and higher
- Implement the interface on Android 3.1 up to Android 4.0
- Use the version-specific implementation

##### 8.10.4 Support multiple game controllers

- Map players to controller device IDs
- Process multiple controller input

#### 8.11 Work with input method editors (IMEs)

##### 8.11.1 Create an input method

- The IME lifecycle
- Declare IME components in the manifest
- The input method API
- Design the input method UI
    - Input view
    - Candidates view
    - UI design considerations
- Send text to the application
    - Edit the text around the cursor
    - Support composing text before committing
    - Intercept hardware key events
- Create an IME subtype
    - Choose IME subtypes from the notification bar
    - Choose IME subtypes from System Settings
- Switch among IME subtypes
- General IME considerations

##### 8.11.2 Image keyboard support

- How it works
- Add image support to apps
- Add image support to IMEs

#### 8.12 Spell checker framework

- Spell checker lifecycle
- Implement a spell checker service
    - Spell checker classes
    - Spell checker manifest and metadata
- Access the spell checker service from a client

---

#### 9. Add notification to your app

#### 9.1 Notifications overview

- Appearances on a device
    - Status bar and notification drawer
    - Heads-up notification
    - Lock screen
    - App icon badge
    - Wear OS devices
- Notification anatomy
    - Notification actions
    - Expandable notification
- Notification updates and groups
- Notification channels
- Notification importance
- Do Not Disturb mode
- Notifications for foreground services
- Post limits
- Notification compatibility

#### 9.2 Notification runtime permission

- Declare the permission
- App capabilities depend on user choice in permissions dialog
    - User selects "Allow"
    - User selects "Don't allow"
    - User swipes away from dialog
- Effects on newly-installed apps
- Effects on updates to existing apps
- Eligibility for permission pre-grant
- Exemptions
    - Media sessions
    - Apps configured to self-manage phone calls
- Test your app
- Best practices
    - Update your app's target SDK version
    - Wait to show notification permission prompt
    - Request the permission in context
    - Check whether your app can send notifications
    - Use the permission responsibly

#### 9.3 Create and manage notification channels

- Create a notification channel
    - Set the importance level
- Read notification channel settings
- Open the notification channel settings
- Delete a notification channel
- Create a notification channel group

#### 9.4 Create a notification

##### 9.4.1 Basic Notifications

- Add the AndroidX Core Library
- Create a basic notification
    - Declare the runtime permission
    - Set the notification content
    - Create a channel and set the importance
    - Set the notification's tap action
    - Show the notification
- Add action buttons
- Add a direct reply action
    - Add the reply button
    - Retrieve user input from the reply
- Add a progress bar
- Set a system-wide category
- Show an urgent message
- Set lock screen visibility
- Update a notification
- Remove a notification
- Best practices for messaging apps

##### 9.4.2 Create an expandable notification

- Add a large image
- Add a large block of text
- Create an inbox-style notification
- Show a conversation in a notification
- Create a notification with media controls

##### 9.4.3 Create a call style notification for call apps

- Incoming call
- Ongoing call
- Screen a call
- Provide compatibility across more Android versions

##### 9.4.4 Display time-sensitive notifications

- Add the POST_NOTIFICATIONS permission
- Create a notification channel
- Manage notifications permissions
- Create a high-priority notification
- Display the notification to the user
- Ongoing notification

##### 9.4.5 Create a custom notification layout

- Create custom layout for the content area
    - Prepare the layouts
    - Build and show the notification
- Create a fully custom notification layout

#### 9.5 Create a group of notifications

- Create a group and add a notification to it
- Set a group summary
- Automatic grouping

#### 9.6 Start an Activity from a Notification

- Set up a regular activity PendingIntent
    - Define your app's Activity hierarchy
    - Build a PendingIntent with a back stack
- Set up a special activity PendingIntent

#### 9.7 Add conversations

##### 9.7.1 People and conversations

- Conversation space
- Conversations in Bubbles
- Conversation Shortcuts
- API guidelines
    - Shortcuts for Conversations
    - Conversation Notifications
    - Use LocusIdCompat
- Conversation space requirements for apps that target Android 10 or lower
    - Fallback: If MessagingStyle is used but no shortcut is provided
    - Fallback: If MessagingStyle isn't used, but the app is a recognized messaging app
- Guidance, usage, and testing
    - When should I use conversations?
    - Best practices
    - Testing Conversation Notifications and shortcuts
    - Conversation Widgets

##### 9.7.2 Use bubbles to let users participate in conversations

- The bubble API
    - Create an expanded bubble
    - Bubble content lifecycle
- When bubbles appear
- Best practices

#### 9.8 Modify a notification badge

- Disable badging
- Set custom notification count
- Modify a notification's touch & hold menu icon
- Hide a duplicate shortcut

#### 9.9 Show pop-up messages

##### 9.9.1 Pop-up messages overview

##### 9.9.2 Build and display a pop-up message

- Use a CoordinatorLayout
- Display a message
    - Create a Snackbar object
    - Show the message to the user

##### 9.9.3 Add an action to a message

---

#### 10. Customize app launch

#### 10.1 Adaptive icons

- Design adaptive icons
- Add your adaptive icon to your app

#### 10.2 Add a splash screen

##### 10.2.1 Splash screens

- How the splash screen works
- Elements and mechanics of the splash screen
    - Splash screen dimensions
    - Splash screen animations and the launch sequence
    - Splash screen resources

##### 10.2.2 Migrate your splash screen implementation to Android 12 and later

- SplashScreen compat library
- Migrate your splash screen implementation
- Adapt your custom splash screen Activity to the splash screen
    - Prevent the custom Activity from being displayed
    - Keep the custom activity for branding
    - Remove the custom splash screen Activity

#### 10.3 Add app shortcuts

##### 10.3.1 App shortcuts overview

- Shortcut types
- Display shortcuts in assistants using capabilities
- Shortcut limitations

##### 10.3.2 Create shortcuts

- Create static shortcuts
    - Customize attribute values
    - Configure inner elements
- Create dynamic shortcuts
    - Add the Google Shortcuts Integration Library
- Create pinned shortcuts
    - Create a custom shortcut activity
- Test shortcuts

##### 10.3.3 Add capabilities to shortcuts

- Define capabilities in shortcuts.xml
- Associate shortcuts with a capability

##### 10.3.4 Manage shortcuts

- Shortcut behavior
    - Shortcut visibility
    - Shortcut display order
- Manage multiple intents and activities
    - Assign multiple intents
    - Start one activity from another
    - Set intent flags
- Update shortcuts
    - Handle system locale changes
    - Track shortcut usage
- Disable shortcuts
- Rate limiting
- Backup and restore

##### 10.3.5 Best practices for shortcuts

---

#### 11. Add app content to the home screen or launcher

#### 11.1 Create custom Quick Settings tiles for your app

- Decide when to create a tile
- Create your tile
    - Create your custom icon
    - Create and declare your TileService
- Manage your TileService
    - TileService lifecycle overview
    - Select a listening mode
    - Tile states overview
    - Update your tile
    - Handle taps
    - Mark your tile as toggleable
    - Perform only safe actions on securely-locked devices
- Prompt the user to add your tile

#### 11.2 Create app widgets

##### 11.2.1 App widgets overview

- Widget types
    - Information widgets
    - Collection widgets
    - Control widgets
    - Hybrid widgets
- Integrate widgets with Google Assistant
- Widget limitations
    - Gestures
    - Elements
- Design guidelines
    - Widget content
    - Widget navigation
    - Widget resizing
    - Layout considerations
    - Widget configuration by users
- Widget design checklist

##### 11.2.2 Create a simple widget

- Widget components
- Declare the AppWidgetProviderInfo XML
    - Widget sizing attributes
    - Additional widget attributes
- Use the AppWidgetProvider class to handle widget broadcasts
    - Declare a widget in the manifest
    - Implement the AppWidgetProvider class
    - Receive widget broadcast intents
- Create the widget layout
    - Support for stateful behavior
- Implement rounded corner

##### 11.2.3 Enhance your widget

- Use dynamic colors
    - Backward compatibility for dynamic colors
- Enable voice support
- Improve your app's widget picker experience
    - Add scalable widget previews to the widget picker
    - Recommended approaches for building accurate previews
    - Backward compatibility with scalable widget previews
- Add a description for your widget
- Enable smoother transitions
- Use runtime modification of RemoteViews

##### 11.2.4 Create an advanced widget

- Optimizations for updating widget content
    - Types of widget updates
    - Determine how often to update a widget
    - Considerations when updating a widget from a BroadcastReceiver
- Build accurate previews that include dynamic items
    - Complex list items

##### 11.2.5 Use collection widgets

- Sample application
- Implement widgets with collections
    - Manifest for widgets with collections
    - Layout for widgets with collections
    - AppWidgetProvider class for widgets with collections
- Persist data
    - RemoteViewsFactory interface
    - Add behavior to individual items
- Keep collection data fresh
- Use RemoteCollectionItems to pass along a collection directly

##### 11.2.6 Provide flexible widget layouts

- Use improved APIs for widget sizes and layouts
    - pecify additional widget sizing constraints
    - Provide responsive layouts
    - Provide exact layouts
- Determine a size for your widget

##### 11.2.7 Enable users to configure app widgets

- Declare the configuration activity
- Implement the configuration activity
    - Update the widget from the configuration activity
- Widget configuration options
    - Enable users to reconfigure placed widgets
    - Use the widget's default configuration
- Let users pin a widget

##### 11.2.8 Build a widget host

- Binding widgets
- Host responsibilities
    - Determine your approach based on the targeted Android version

##### 11.2.9 Integrate content with home channels

###### **11.2.9.1 Engage SDK**

###### **11.2.9.2 Engage SDK Read: Third-party technical integration instructions**

- Integration detail
    - Terminology
    - Pre-work
    - Summary
    - Step 1: Provide entity data
    - Step 2: Provide Cluster data
    - Step 3: Handle broadcast intents
- Integration workflow

###### **11.2.9.3 Engage SDK Watch: Third-party technical integration instructions**

- Integration detail
    - Terminology
    - Pre-work
    - Summary
    - Step 0: Migration from existing Media Home SDK integration
    - Step 1: Provide entity data
    - Step 2: Provide Cluster data
    - Step 3: Handle broadcast intents
- Integration workflow

###### **11.2.9.4 Engage SDK Listen: Third-party technical integration instructions**

- Integration detail
    - Terminology
    - Pre-work
    - Summary
    - Step 1: Provide entity data
    - Step 2: Provide Cluster data
    - Step 3: Handle broadcast intents
- Integration workflow

##### 11.2.10 Control external devices

- User interface
- Create the service
    - Declare the service
    - Select the correct control type
    - Create publishers for the controls
    - Handle actions

---

#### 12. Create backward-compatible UIs

#### 12.1 About backward-compatible UIs

#### 12.2 Abstract the new APIs

- Prepare for abstraction
- Create an abstract tab interface
- Abstract ActionBar.Tab
- Abstract ActionBar tab methods

#### 12.3 Proxy to the new APIs

- Implement tabs using new APIs
- Implement CompatTabHoneycomb
- Implement TabHelperHoneycomb

#### 12.4 Create an implementation with older APIs

- Decide on a substitute solution
- Implement tabs using older APIs

#### 12.5 Use the version-aware component

- Add the switching logic
- Create a version-aware activity layout
- Use TabHelper in your activity
