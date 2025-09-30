# Language Translation Tool

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Saadumar26/codealpha_translation_tool/blob/main/Language_Translation_Tool.ipynb)
&nbsp;
![Python Version](https://img.shields.io/badge/python-3.x-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

A powerful and user-friendly Language Translation Tool that runs directly in a Jupyter Notebook or Google Colab environment. This tool provides a seamless interface for translating text between a multitude of languages, complete with text-to-speech functionality to listen to the translated output.

## Features

-   **Interactive UI in Jupyter/Colab:** Built with `ipywidgets` to create a rich, interactive user experience without needing a separate web application.
-   **Multi-Language Support:** Translate text to and from any of the languages supported by Google Translate.
-   **Auto Language Detection:** Automatically detect the source language of the input text.
-   **Text-to-Speech:** Listen to the translated text with the click of a button, thanks to the Google Text-to-Speech (gTTS) integration.
-   **Copy to Clipboard:** Easily copy the translated text for use in other applications.
-   **User-Friendly Design:** Includes features like a "Clear" button to reset the tool, status messages to provide feedback, and sorted language lists with popular languages prioritized for quick access.

## Tech Stack

-   **Backend:** Python
-   **Translation API:** `googletrans` - a free and unlimited Python library that implements the Google Translate API.
-   **Text-to-Speech:** `gTTS` (Google Text-to-Speech) - a Python library to interface with Google Translate's text-to-speech API.
-   **Interactive UI:** `ipywidgets` - for creating interactive HTML widgets in Jupyter notebooks.

## Getting Started

You can run this project in two ways:

### 1. Run with Google Colab (Recommended)

Click the "Open in Colab" badge at the top of this README to open the notebook directly in Google Colab.

### 2. Run on a Local Machine

Follow these instructions to get a copy of the project up and running on your local machine.

#### Prerequisites

-   Python 3.x
-   Jupyter Notebook or JupyterLab

#### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Saadumar26/codealpha_translation_tool.git
    cd codealpha_translation_tool
    ```

2.  **Install the required Python libraries:**
    ```bash
    pip install ipywidgets googletrans==4.0.0-rc1 gTTS
    ```
    *Note: It's recommended to install this specific version of `googletrans` for better stability.*

## Usage

1.  **Launch the Tool:**
    -   Open the `Language_Translation_Tool.ipynb` file in your chosen environment (Colab, Jupyter Notebook, or JupyterLab).
    -   Run all the cells. The interactive translation tool will appear.

2.  **Translate Text:**
    -   **Enter Text:** Type or paste the text you want to translate into the "Input" text area.
    -   **Select Languages:**
        -   Choose the source language from the "From" dropdown, or leave it as "Auto-detect".
        -   Select the desired target language from the "To" dropdown.
    -   **Translate:** Click the "🔄 Translate" button. The translated text will appear in the output area below.

3.  **Use Additional Features:**
    -   **Listen:** Click the "🔊 Listen" button to hear an audio playback of the translated text.
    -   **Copy:** Click the "📋 Copy Translation" button to copy the text to your clipboard.
    -   **Clear:** Click the "🗑️ Clear" button to reset all fields and start a new translation.

## How It Works

The tool is built using several Python libraries that work together to provide a seamless experience:

-   **`ipywidgets`**: This library is used to create all the UI components, such as the text area, dropdowns, and buttons, and to arrange them in a clean layout within the notebook.
-   **`googletrans`**: This is the core translation engine. When you click the "Translate" button, the input text is sent to the Google Translate API via this library. It handles both the translation and the auto-detection of the source language.
-   **`gTTS` (Google Text-to-Speech)**: When the "Listen" button is clicked, the translated text is passed to the `gTTS` library. It communicates with Google's text-to-speech service to generate an MP3 audio file of the text being spoken in the target language. This audio is then embedded directly into the notebook for playback.

## Contributing

Contributions are welcome! If you have ideas for improvements or want to fix a bug, please feel free to:

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.
