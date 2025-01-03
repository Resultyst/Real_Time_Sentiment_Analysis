# Real-Time AI-Powered Sales Intelligence Tool

![Project Banner](<!-- Add a banner image URL here -->)

Real-Time AI-Powered Sales Intelligence Tool is a cutting-edge application designed to assist sales teams during live sales calls by providing real-time insights and suggestions. The tool leverages advanced AI models (e.g., Mixtral, LLaMA) to analyze conversations, detect sentiment, and provide actionable recommendations to improve sales outcomes.

## Features

- **Real-Time Sentiment Analysis**: Detects the sentiment of the conversation (Positive, Negative, Neutral, etc.).
- **Emotion Detection**: Identifies the emotional state of the buyer (Excitement, Frustration, etc.).
- **Buyer Engagement Analysis**: Assesses the level of buyer engagement (Low, Moderate, High).
- **Purchase Intent Analysis**: Classifies the buyer's purchase intent (Immediate, Exploratory, etc.).
- **Behavioral Intent Analysis**: Identifies behavioral intent signals (Website browsing, Cart abandonment, etc.).
- **Advanced Intent Detection**: Detects advanced intent markers (High-value lead identification, etc.).
- **Integration with CRM and Google Sheets**: Stores and analyzes data for future reference (# Currently working on this part)

## Demo

<!-- Add a GIF or video demo of your project in action -->

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [API Documentation](#api-documentation)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Acknowledgments](#acknowledgments)

## Installation

### Prerequisites

- Python 3.x
- Node.js (for frontend dependencies, if applicable)
- Groq API Key (Sign up at [Groq](https://www.groq.com))

### Steps

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/real-time-sales-intelligence-tool.git
    cd real-time-sales-intelligence-tool
    ```

2. Set up the backend:

    ```bash
    pip install -r requirements.txt
    ```

3. Set up the frontend:

    - Serve the `index.html` file using a web server (e.g., Nginx, Apache).

4. Set environment variables:

    - Create a `.env` file in the root directory and add your Groq API key:

      ```env
      GROQ_API_KEY=your_groq_api_key_here
      ```

5. Run the Flask app:

    ```bash
    python app.py
    ```

6. Open the application in your browser:

    ```
    http://localhost:5000
    ```

## Usage

1. Open the application in a supported browser.
2. Click **Start Recording** to begin speech recognition.
3. Speak into the microphone during a sales call.
4. View real-time insights (sentiment, emotion, engagement, etc.) on the dashboard.
5. Click **Stop Recording** to end the session.
6. Save the transcription and analysis results to an Excel file.

## API Documentation

### Endpoint: `/get_response`

- **Method**: POST
- **Request Body**:

    ```json
    {
      "user_input": "Transcribed text from the user"
    }
    ```

- **Response Body**:

    ```json
    {
      "response": "User input",
      "sentiment": "Positive",
      "emotion": "Excitement",
      "engagement": "High",
      "purchase_intent": "Immediate purchase intent",
      "behavioral_intent": "Website browsing intent",
      "advanced_intent": "High-value lead identification",
      "suggestions": "Suggestions based on the input"
    }
    ```

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository.
2. Create a new branch:

    ```bash
    git checkout -b feature/your-feature-name
    ```

3. Commit your changes:

    ```bash
    git commit -m "Add your feature"
    ```

4. Push to the branch:

    ```bash
    git push origin feature/your-feature-name
    ```

5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.

## Contact

For questions or feedback, feel free to reach out:

- **Email**: your-email@example.com
- **GitHub**: [your-username](https://github.com/your-username)
- **LinkedIn**: [Your Name](https://www.linkedin.com/in/your-name)

## Acknowledgments

- **Groq** for providing the AI API.
- **Flask** for the backend framework.
- **Tailwind CSS** for the frontend styling.