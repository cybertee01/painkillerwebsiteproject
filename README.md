# Voice Assistant Website Integration

This project is a web application that integrates an interactive AI voice assistant powered by Vapi alongside a WhatsApp messaging widget. The primary goal of the design is to provide visitors with immediate voice and text support channels without cluttering the screen or causing visual overlap between interactive elements. The site is hosted on GitHub and configured for automated continuous deployment using Netlify.

## Overview and Functionality

The application uses standard HTML, JavaScript, and CSS for its structure and styling. The Vapi voice widget script is embedded near the bottom of the main HTML file to ensure that page markup loads completely before the voice integration initializes. To prevent interface collision with the existing WhatsApp widget positioned in the bottom-right corner, the Vapi assistant is configured to anchor to the bottom-left area of the viewport.

## Project Structure

The codebase is organized into a few core files:

index.html contains the primary layout, user interface elements, and embedded script tags for both Vapi and WhatsApp.

netlify.toml manages the build and deployment parameters for hosting on Netlify.

README.md provides project context and documentation.

## Setup and Configuration

To run or modify this project locally, clone the repository to your local machine using git clone with your repository URL. Open index.html in your code editor and scroll to the script tag located just above the closing body tag.

To connect your own voice assistant, replace the placeholder strings inside the script initialization with your actual keys from the Vapi dashboard. Set the apiKey parameter to your public key and the assistant parameter to your specific assistant ID. Ensure both strings remain inside quotation marks and retain the trailing commas to keep the JavaScript syntax valid.

## Deployment Process

This repository is connected directly to Netlify for continuous integration. Any commits pushed or merged into the main branch automatically trigger a fresh site build on Netlify, updating the live deployment within a few minutes.

```
