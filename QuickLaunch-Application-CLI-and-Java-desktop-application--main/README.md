# Bash_automation-and-QuickLaunch-app

## Overview
QuickLaunch is a startup application designed to automate the launch of frequently used commands and links. It provides both a graphical user interface (GUI) and a command-line interface (CLI) to streamline your workflow. This application can be configured to start automatically on boot and is compatible with both Linux and Windows operating systems.

## Features
Graphical User Interface (JavaFX)

Easily add and manage options consisting of commands and links.
Execute selected options with a double-click or by pressing the 'Enter' key.
Edit or delete existing options through a user-friendly interface.
The application icon and styles are customizable.
Command-Line Interface (Bash Script)

Quickly execute predefined commands and open links directly from the terminal.
Simple and efficient, designed for users who prefer the command line.
Cross-Platform Compatibility

The JavaFX application works on both Linux and Windows.
The Bash script is tailored for Linux environments.

## Setup Instructions
### Requirements
* JavaFX SDK: Ensure you have JavaFX SDK installed.
* Java Runtime Environment (JRE): Required for running the Java application.
* Bash: Required for running the CLI on Linux.

### Installation
#### Clone the Repository:
```
    git clone <repository-url>
    cd QuickLaunch_application
```

#### JavaFX Application:

Compile the Java application:

``` 
    javac --module-path path/to/javafx-sdk-22/lib --add-modules javafx.controls Main.java Option.java 
```

Run the application:

``` 
    java --module-path path/to/javafx-sdk-22/lib --add-modules javafx.controls Main 
```

#### Bash CLI:

Make the script executable:
```
    chmod +x quicklaunch.sh
```

Run the script:
```
    ./quicklaunch.sh
```

#### Set Up as a Startup Application (Linux):

Create a .desktop file in ~/.config/autostart/:

```
    [Desktop Entry]
    Type=Application
    Exec=/home/shreyash/Projects/Bash_automation_And_QuickLaunch_application/QuickLauch_application/quicklaunch.sh
    Hidden=false
    NoDisplay=false
    X-GNOME-Autostart-enabled=true
    Name=QuickLaunch Application
    Comment=Start the QuickLaunch Java application on login
    Icon=/home/shreyash/Projects/Bash_automation_And_QuickLaunch_application/QuickLauch_application/Quick.jpeg`
```

### Usage
#### JavaFX Application:

Launch the application, add your frequently used commands and links, and execute them with ease.
#### Bash CLI:

Run ./quicklaunch.sh to quickly execute predefined commands or open links.
### Customization
* Icon and Styles: Customize the application's icon by changing the Icon field in the .desktop file.
* Modify the styles.css file to adjust the appearance of the JavaFX application.
* Edit bash script for custom options.
