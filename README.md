![Tweeter Logo](TweeterLogo.png)


# 🐦 Tweeter – Social Network Interface

Tweeter is a simulated social media platform that allows for user management, post creation, following systems, and feed recommendation logic.  
This interface provides a command-line style interaction with the database and supports various user and account operations.

---

## 📋 Available Commands

Each command follows this format:  
**`command_name {arguments}`** – *Description*

---

### 🛠️ System Initialization

- **`create {}`**  
  Initializes the database and its schema. No user or post data is added yet.

- **`generate {}`**  
  Fills the database with:
  - Random users
  - Follows
  - Subscriptions
  - Blocks

---

### 👤 User & Account Management

- **`adduser {email}`**  
  Registers a new user by their email.

- **`addaccount {email, username, password}`**  
  Creates a new account for the given email with a specified username and password.

- **`followAccount {followerUsername, followeeUsername}`**  
  Makes one account follow another.

- **`unfollowAccount {unfollowerUsername, unfolloweeUsername}`**  
  Unfollows the specified account.

- **`listUsers {}`**  
  Displays a list of all registered users.

- **`listAccounts {}`**  
  Displays a list of all created accounts.

---

### 📝 Post Operations

- **`createPost {username, content, image, hashtag}`**  
  Creates a new post with:
  - Text content
  - An image filename
  - A hashtag

- **`editPost {content, image, hashtag, post_id}`**  
  Updates a post by its `post_id` with new content, image, and hashtag.

- **`deletePost {post_id}`**  
  Deletes a post using its ID.

---

### 📰 Feed & Recommendations

- **`displayFeed {account_id}`**  
  Displays posts from accounts followed by the given account.

- **`displayRecommendedFollowees {account_id}`**  
  Recommends accounts to follow based on mutual connections and scoring.

- **`displayRecommendedFeed {account_id}`**  
  Shows posts from recommended followees.

---

### 📊 Analytics

- **`subscriberScore {}`**  
  Calculates a score for each account based on their subscription-to-following ratio.

---

## 📌 Notes

- Command inputs must follow the exact format shown above.
- This project was created for educational purposes to simulate social media backend logic.

---

## 👨‍💻 Author

**Lexi Purser**  
