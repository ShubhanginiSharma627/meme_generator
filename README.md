# Music Generator App

The Music Generator App is a Flutter application that generates and plays AI-generated music based on user prompts and styles. It leverages the `SunoApi` to create music and integrates with `audioplayers` for audio playback. The app features a modern and intuitive interface with a focus on ease of use and performance.

## Features

-   **AI Music Generation**: Create music tracks by providing a description prompt and selecting a music style.
-   **Audio Playback**: Play and pause the generated music directly within the app.
-   **Custom Themes**: Enjoy a visually appealing user interface with a deep purple and indigo theme.
-   **Responsive Design**: The app is optimized for various screen sizes and orientations.
-   **Settings**: Placeholder for future enhancements and custom settings.

## Getting Started

### Prerequisites

-   **Flutter**: Ensure that Flutter is installed on your machine. You can download and install Flutter from the [official website](https://flutter.dev).
-   **API Access**: You need access to the `SunoApi`. Replace the placeholder cookie value with your actual cookie for the API.

### Installation

1. **Clone the Repository**:

    Open your terminal or command prompt and run:

    ```bash
    git clone https://github.com/ShubhanginiSharma627/meme_generator.git
    cd meme_generator
    ```

2. **Install Dependencies**:

    Run the following command to install the required dependencies:

    ```bash
    flutter pub get
    ```

3. **Run the App**:

    You can run the app on an emulator or a physical device using:

    ```bash
    flutter run
    ```

## Project Structure

-   **`lib/`**: Contains the main source code.
    -   **`main.dart`**: The main entry point of the app.
    -   **`api/suno_api.dart`**: Manages API interactions with `SunoApi`.
    -   **`models/song_clip.dart`**: Defines the data model for song clips.
-   **`pubspec.yaml`**: Contains the project's dependencies and asset declarations.

## Key Components

### `MyApp`

-   The main class that sets up the `MaterialApp`.
-   Configures global theming with a deep purple and indigo color scheme.

### `MusicGeneratorScreen`

-   The main screen where users can input prompts and music styles.
-   Displays a list of generated songs and includes controls for playing and pausing music.
-   Manages the state for loading, playing, and stopping music.

### `SongCard`

-   A widget that represents an individual music track.
-   Displays the track's image, title, and tags, and includes a play/pause button.

### `SunoApi`

-   Handles API interactions for generating and retrieving music.
-   Includes methods for fetching authentication tokens and checking for audio URLs.

## Usage

1. **Enter a Prompt**: Type a description for the music you want to generate in the 'Enter prompt' field.
2. **Enter a Music Style**: Specify the music style you prefer in the 'Enter music style' field.
3. **Generate Music**: Click the 'Generate Song' button to create music based on your inputs.
4. **Play Music**: Use the play button on the song card to listen to the generated track.

## Configuration

-   **API Integration**: Update the `SunoApi` class with your actual API credentials and cookies.
-   **Custom Fonts**: Add your desired fonts to the `pubspec.yaml` file and update the font family in `main.dart`.

## Dependencies

-   **`audioplayers`**: For audio playback functionality.
-   **`flutter/material.dart`**: Core Flutter framework for UI design.
-   **`google_fonts`**: To use Google Fonts within the app.
-   **`http`**: For making HTTP requests to the `SunoApi`.

## Troubleshooting

-   **API Errors**: Ensure that your API credentials are correct and the API service is accessible.
-   **Playback Issues**: Verify that the audio URLs are valid and accessible.
-   **UI Problems**: Check that all assets and fonts are correctly linked in the `pubspec.yaml`.

## Future Enhancements

-   **Settings Page**: Implement a settings page for more user customization options.
-   **Offline Playback**: Enable the downloading of tracks for offline listening.
-   **Improved UI**: Add animations and refine the user interface for a better experience.
