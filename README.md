# Lectures

Welcome to my **Lectures** repository! This project is the backend for how I build and deploy all of my educational materials from Markdown. Below, you'll find information on how to access and utilize the contents of this repository. Some aspects are tailored for my needs but most are generally applicable.

## Overview

This repository contains a collection of lecture materials, including slides and related resources, aimed at facilitating learning and teaching all generated from Markdown files using [Slidev](https://github.com/slidevjs/slidev). The materials are organized into different sections for easy navigation and to allow for selective updating due to content changes.

## Getting Started

To host your own slides using this repository, follow these steps:

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/ChristopherWMM/lectures.git
   ```

2. **Navigate to the Repository**:

   ```bash
   cd lectures
   ```

3. **Install Dependencies**:

   Ensure you have [Node.js](https://nodejs.org/) installed. Then, install the necessary packages:

   ```bash
   npm install
   ```

4. **Create a slideshow using Slidev**:

   Initialize a new Slidev project:

   ```bash
   npx slidev init your/lecture/path
   cd your/lecture/path
   ```

   Note: Whatever file path you choose will determine the url created for the lecture on the generated `index.html` page.

5. **Preview your slideshow**:

   Run the development server to preview your slides:

   ```bash
   npx slidev
   ```

6. **Deploy**:

   Commit and push your changes to automatically build and deploy your slides!

   They are viewable at the following url: `<your_GitHub_username>.github.io/lectures`

   Note: Changing the name of this repository will change the root page of where the slides are located at.

## Repository Structure

The repository is structured as follows:

- `common/`: Contains individual Slidev elements that are reused across multiple projects.
- `published/`: Includes the Slidev projects automatically built and deployed.
- `wip/`: Contains wip Slidev projects still under development.
- `index.css`: Stylesheet used on the generated nagivational lecture page.
- `package.json` & `package-lock.json`: Manage project dependencies.

## Contact

For any questions or suggestions, please open an issue in this repository.

---

Thank you for your interest in my lectures repository! Hopefully this helps you better your prep workflow!