# Dice Roller App

A simple and interactive dice rolling application built with Jetpack Compose. This app allows users to simulate rolling a six-sided die with a tap of a button.

<img width="230" src="https://github.com/user-attachments/assets/c6680c54-f9fc-4d9e-8bbd-34572b8e8cb1"/>


## Features

- Clean and intuitive user interface
- Realistic dice images for each roll
- Smooth animations and transitions
- Material Design 3 components
- Edge-to-edge display support

## Technical Specifications

### Built With
- Kotlin 1.9.0
- Jetpack Compose 2024.04.01
- Material Design 3
- Android Edge-to-Edge UI

### Dependencies

```toml
# Core Dependencies
androidx-core-ktx = "1.12.0"
lifecycle-runtime-ktx = "2.8.7"
activity-compose = "1.9.3"

# Compose BOM
compose-bom = "2024.04.01"

# Testing Dependencies
junit = "4.13.2"
androidx-junit = "1.2.1"
espresso-core = "3.6.1"

# Build Tools
android-gradle-plugin = "8.5.0"
```

### Key Components

#### MainActivity
The main entry point of the application that sets up the theme and scaffold structure.

#### DiceRollerApp Composable
The main composable function that handles:
- State management for dice rolls
- UI layout and composition
- User interactions
- Image resource management

### UI Elements

1. **Header**
   - App title using Serif font family
   - Bold text with 36sp size
   - Center-aligned text

2. **Dice Display**
   - Dynamic image loading based on roll result
   - Six different dice face images (dice_1 through dice_6)
   - Centered positioning with padding

3. **Roll Button**
   - Custom styled with teal background
   - Yellow border with 1dp width
   - Rounded corners (8dp radius)
   - Customized button colors
   - Localized "Roll" text

## State Management

The app uses Jetpack Compose's `mutableIntStateOf` to manage the current dice value:
```kotlin
var result by remember { mutableIntStateOf(1) }
```

## Design Choices

- **Layout**: Uses a Column composable with center alignment
- **Spacing**: Strategic use of Spacer composables for proper element distribution
- **Theme**: Custom theme implementation with DiceRollerAppTheme
- **Accessibility**: Content descriptions for image resources
- **Preview**: Includes preview composable for development

## Getting Started

1. Clone the repository
2. Open in Android Studio
3. Run on an emulator or physical device

## Requirements

- Android Studio Arctic Fox or newer
- Kotlin 1.9.0 or higher
- Minimum SDK version: [Add your minimum SDK version]
- Target SDK version: [Add your target SDK version]
- Gradle Plugin Version: 8.5.0

## Development Setup

### Gradle Dependencies

The project uses the following key dependencies:

```kotlin
// Core Android dependencies
implementation("androidx.core:core-ktx:1.12.0")
implementation("androidx.lifecycle:lifecycle-runtime-ktx:2.8.7")
implementation("androidx.activity:activity-compose:1.9.3")

// Compose dependencies
implementation(platform("androidx.compose:compose-bom:2024.04.01"))
implementation("androidx.compose.ui:ui")
implementation("androidx.compose.ui:ui-graphics")
implementation("androidx.compose.ui:ui-tooling-preview")
implementation("androidx.compose.material3:material3")

// Testing dependencies
testImplementation("junit:junit:4.13.2")
androidTestImplementation("androidx.test.ext:junit:1.2.1")
androidTestImplementation("androidx.test.espresso:espresso-core:3.6.1")
```


## Acknowledgments

- Material Design guidelines
- Jetpack Compose documentation
- Android Edge-to-Edge UI guidelines
