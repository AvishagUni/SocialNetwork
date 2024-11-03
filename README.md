# Social Network Simulation with Design Patterns

This project is a Python-based simulation of a social network, implementing essential design patterns to manage users, posts, and interactions. The social network allows users to connect, post updates, and interact with each other, showcasing how object-oriented principles and design patterns can be applied in a real-world scenario.

---

## 📋 Project Overview

The core functionality of the social network includes:

1. **User Management**: Registering and managing user connections (followers).
2. **Post Interactions**: Users can create posts, like, and comment on others' posts.
3. **Notifications**: Users receive notifications when they get new followers, comments, or likes.
4. **Post Types**: Supports three types of posts, each with specific attributes:
   - **TextPost**: Standard text-based post.
   - **ImagePost**: Contains a path to an image file and can display it.
   - **SalePost**: Lists an item for sale, including item description, price, and availability status.

---

## 🛠 Design Patterns

The project uses the following design patterns to structure and organize the code:

- **Singleton**: Ensures only one instance of the social network exists at any time.
- **Observer**: Manages notifications for followers about posts and interactions.
- **Factory**: Creates different types of posts (TextPost, ImagePost, SalePost) based on user input.

---

## 📂 Project Structure

- `main.py`: The main script to run the simulation, containing test cases and example usage.
- `auto_check.py`: A script for automatic testing, comparing the program's output to the expected output in `output.txt`.
- `output.txt`: Expected output for validation against program results.
- Additional files: Class and function implementations for users, posts, and design patterns.

---

## 🔧 Features

1. **User Registration and Authentication**
   - Register new users with a username and password.
   - Enforce unique usernames and password length constraints.
   - Users can log in and log out, affecting their ability to post and interact.

2. **Follow and Unfollow**
   - Users can follow or unfollow others, receiving notifications for new posts from followed users.

3. **Posting and Interactions**
   - Users can create text, image, and sale posts.
   - Each post type has unique properties:
     - **TextPost**: Displays plain text.
     - **ImagePost**: Shows an image using `matplotlib`.
     - **SalePost**: Allows setting a price, applying discounts, and marking items as sold.
   - Users can like and comment on posts.

4. **Notifications**
   - Followers are notified of new posts, comments, and likes.
   - Users can view a log of all notifications, ordered from oldest to newest.

5. **Testing and Output Validation**
   - Run `auto_check.py` to compare your program’s output with `output.txt`.
   - Ensure the program output matches `output.txt` for accurate results.

---

## 🚀 Getting Started

### Requirements
- Python 3
- `matplotlib` library for image display in ImagePost

### Installation
Clone the repository and install required dependencies:
```bash
git clone https://github.com/yourusername/social-network-simulation.git
cd social-network-simulation
pip install -r requirements.txt
