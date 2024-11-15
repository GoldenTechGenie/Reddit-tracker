# Reddit Stats Tracker

Reddit Stats Tracker is a Golang-based application that monitors real-time statistics from a chosen subreddit. It provides insights into the most engaging posts and active users while maintaining efficiency and adhering to Reddit's API rate limits.

## Features

- **Track Top Posts:** Identifies and logs the highest upvoted posts.
- **Monitor Active Users:** Highlights users with the most contributions in the subreddit.
- **Real-Time Data Processing:** Fetches and processes large volumes of posts concurrently.
- **Rate Limit Friendly:** Operates within Reddit API rate limit constraints using efficient data handling techniques.

## Technologies

- **Golang:** Core programming language.
- **Reddit API:** For accessing subreddit data.
- **Logrus:** Enables structured and detailed logging.
- **Goroutines & Channels:** Implements concurrency for efficient data processing.
- **godotenv:** Simplifies environment variable management.

## Getting Started

### Prerequisites

Ensure you have the following installed:

- **Golang** (1.18 or later)
- A Reddit API application with valid credentials ([Reddit API Documentation](https://www.reddit.com/dev/api/))

### Setup Instructions

1. **Configure Environment Variables**
   - Create a `.env` file in the root of the project with your Reddit API credentials:
     ```env
     REDDIT_CLIENT_ID=your_client_id
     REDDIT_CLIENT_SECRET=your_client_secret
     REDDIT_USERNAME=your_username
     REDDIT_PASSWORD=your_password
     ```

2. **Install Dependencies**
   - Download and install required dependencies:
     ```bash
     go mod tidy
     ```

3. **Run the Application**
   - Start the tracker:
     ```bash
     go run main.go
     ```

The application will begin fetching and logging statistics from the specified subreddit.

## Contribution

Contributions are welcome! Feel free to submit a pull request or open an issue for any suggestions or improvements.

---

**License:** This project is licensed under the [MIT License](LICENSE). 

For any inquiries or feedback, feel free to contact the repository maintainer.
