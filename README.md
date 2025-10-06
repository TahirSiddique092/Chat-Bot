# Sri Sapthagiri College Chatbot: A Comprehensive Guide

Welcome to the official chatbot of Sri Sapthagiri Pre-University College! This guide will walk you through the process of setting up and running this chatbot on your local machine. Whether you're a seasoned developer or just starting, this guide will provide you with all the necessary steps to get the chatbot up and running.

## Project Overview

This chatbot is designed to be a virtual assistant for Sri Sapthagiri Pre-University College. It can provide information about the college, including courses, faculty, events, and more. The goal of this project is to provide a user-friendly and interactive way for students, parents, and staff to get the information they need.

## Features in Detail

*   **Course Information:** Get details about the science and commerce streams offered at the college, including the different subject combinations available.
*   **Faculty Information:** Learn more about the esteemed faculty members of the college, including their qualifications and departments.
*   **Event Information:** Stay up-to-date with the latest events happening at the college, from the STEM Expo to cultural fests.
*   **College Information:** Get answers to frequently asked questions about the college, such as its location, history, and special achievements.
*   **Conversational AI:** Engage in a natural and interactive conversation with the chatbot.

## Getting Started - The Ultimate Guide

This guide will provide you with a step-by-step process to set up the chatbot on your local machine. We'll cover everything from setting up the environment to running the chatbot.

### Prerequisites

Before you begin, make sure you have the following software installed on your machine:

*   **Python (version 3.8 or higher):** You can download Python from the official website: [https://www.python.org/downloads/](https://www.python.org/downloads/)
*   **pip:** pip is the package installer for Python. It usually comes with Python, but you can check if it's installed by running `pip --version` in your terminal.
*   **Git:** Git is a version control system that we'll use to clone the repository. You can download Git from the official website: [https://git-scm.com/downloads](https://git-scm.com/downloads)

### Setting up the Environment

To avoid conflicts with other Python projects, it's highly recommended to create a virtual environment for this project.

1.  **Create a virtual environment:**
    ```sh
    python -m venv venv
    ```
2.  **Activate the virtual environment:**
    *   **On Windows:**
        ```sh
        .\venv\Scripts\activate
        ```
    *   **On macOS and Linux:**
        ```sh
        source venv/bin/activate
        ```

### Cloning the Repository

Now, let's clone the repository to your local machine.

```sh
git clone https://github.com/Mustaqeem-Rafi/Rasa-Chatbot-Project.git
cd Rasa-Chatbot-Project
```

### Installing Dependencies

Next, we'll install all the required dependencies for this project.

```sh
pip install -r requirements.txt
```

### Understanding the Project Structure

Here's a brief overview of the key files and directories in the project:

*   `actions/`: This directory contains the custom actions for the chatbot.
*   `data/`: This directory contains the NLU data, stories, and rules for the chatbot.
*   `models/`: This directory will contain the trained models.
*   `config.yml`: This file contains the configuration for the NLU pipeline and policies.
*   `domain.yml`: This file defines the intents, entities, slots, responses, and actions for the chatbot.
*   `endpoints.yml`: This file contains the configuration for the action server and other endpoints.

### Training the Model

Now, it's time to train the Rasa model. This will train the NLU model and the Core model.

```sh
rasa train
```

**Note on 2025 Rasa Protocols:** As of 2025, Rasa may have introduced new training commands or options. Always refer to the official Rasa documentation for the latest information on training models.

### Running the Chatbot

To run the chatbot, you'll need to run the Rasa server and the action server in two separate terminals.

**Terminal 1: Run the Rasa Server**

```sh
rasa run
```

**Terminal 2: Run the Action Server**

```sh
rasa run actions
```

Once both servers are running, you can interact with the chatbot through the command line in the first terminal.

## Troubleshooting Common Issues

*   **Dependency Issues:** If you encounter any issues with the dependencies, make sure you are using the correct version of Python and that you have activated the virtual environment.
*   **Model Training Issues:** If you have issues with training the model, make sure your `config.yml` and `domain.yml` files are correctly formatted.
*   **Action Server Issues:** If you have issues with the action server, make sure your `endpoints.yml` file is correctly configured and that your custom actions in the `actions/` directory are free of errors.

## Customization and Extension

*   **Adding New Intents:** To add new intents, you'll need to add them to the `domain.yml` file and provide examples in the `data/nlu.yml` file.
*   **Adding New Responses:** To add new responses, you'll need to add them to the `domain.yml` file.
*   **Adding New Actions:** To add new custom actions, you'll need to create a new action class in the `actions/actions.py` file and add the action to the `domain.yml` file.

## Deployment

This chatbot can be deployed to various platforms, such as a website, Slack, or Facebook Messenger. For detailed instructions on deployment, please refer to the official Rasa documentation.

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

*   The students who developed this chatbot:
    *   Mohammed Tahir
    *   Mustaqeem Rafi
    *   Hema Sai T
    *   Kiran S.K
*   The computer science faculty who guided the project:
    *   Miss Prabharani S
    *   Mr Jeelani