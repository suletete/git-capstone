This Capstone project is a great exercise to practice Git and GitHub workflows while enhancing a community website! Below is a step-by-step guide to simulate the roles of Morgan and Jamie, including creating branches, making changes, and handling pull requests (PRs).

### 1. **Create and Clone Repository**

#### Create Repository on GitHub:
1. Go to GitHub and create a new repository named `greenwood-library-website`.
2. Initialize the repository with a `README.md` file.

#### Clone the Repository to Local Machine:
1. Copy the repository's URL from GitHub.
2. Open your terminal and clone the repository:
   ```bash
   git clone https://github.com/your-username/greenwood-library-website.git
   cd greenwood-library-website
   ```

### 2. **Main Branch Setup (Initial Commit)**

#### Create Basic Files for Web Pages:
1. In the repository, create the following HTML files:
   - `home.html`
   - `about_us.html`
   - `events.html`
   - `contact_us.html`

2. Add some random content into these files. For example:

- `home.html`:
   ```html
   <html>
     <head><title>Home - Greenwood Community Library</title></head>
     <body><h1>Welcome to Greenwood Community Library</h1></body>
   </html>
   ```

- `about_us.html`:
   ```html
   <html>
     <head><title>About Us - Greenwood Community Library</title></head>
     <body><h1>About the Library</h1><p>Greenwood Library is a place for the community to come together and explore knowledge.</p></body>
   </html>
   ```

- `events.html`:
   ```html
   <html>
     <head><title>Events - Greenwood Community Library</title></head>
     <body><h1>Upcoming Events</h1></body>
   </html>
   ```

- `contact_us.html`:
   ```html
   <html>
     <head><title>Contact Us - Greenwood Community Library</title></head>
     <body><h1>Contact Information</h1></body>
   </html>
   ```

#### Stage, Commit, and Push:
1. Stage the changes:
   ```bash
   git add home.html about_us.html events.html contact_us.html
   ```

2. Commit the changes:
   ```bash
   git commit -m "Initial commit with basic website pages"
   ```

3. Push the changes to the `main` branch:
   ```bash
   git push origin main
   ```

---

### 3. **Morgan's Work: Add Book Reviews Section**

#### Create Branch for Morgan:
1. Create a new branch for Morgan:
   ```bash
   git checkout -b add-book-reviews
   ```

#### Add Book Reviews File:
1. Create `book_reviews.html`:
   ```html
   <html>
     <head><title>Book Reviews - Greenwood Community Library</title></head>
     <body><h1>Book Reviews</h1><p>Here are some of our favorite books!</p></body>
   </html>
   ```

#### Stage, Commit, and Push Changes:
1. Stage the new file:
   ```bash
   git add book_reviews.html
   ```

2. Commit the changes:
   ```bash
   git commit -m "Add book reviews section"
   ```

3. Push the branch to GitHub:
   ```bash
   git push origin add-book-reviews
   ```

#### Create a Pull Request for Morgan:
1. Go to the GitHub repository and create a Pull Request (PR) from `add-book-reviews` to `main`.
2. Once the PR is created, review and merge it into the `main` branch.

---

### 4. **Jamie's Work: Update Events Page**

#### Create Branch for Jamie:
1. Create a new branch for Jamie:
   ```bash
   git checkout -b update-events
   ```

#### Update the Events Page:
1. Modify `events.html` to include upcoming community events. For example:
   ```html
   <html>
     <head><title>Events - Greenwood Community Library</title></head>
     <body>
       <h1>Upcoming Events</h1>
       <ul>
         <li>Book Club - April 10, 2025</li>
         <li>Author Talk - April 15, 2025</li>
         <li>Community Picnic - April 20, 2025</li>
       </ul>
     </body>
   </html>
   ```

#### Pull Latest Changes and Stage, Commit, Push:
1. Before proceeding, make sure you have the latest changes from `main`:
   ```bash
   git pull origin main
   ```

2. Stage the changes:
   ```bash
   git add events.html
   ```

3. Commit the changes:
   ```bash
   git commit -m "Update events page with upcoming events"
   ```

4. Push the branch to GitHub:
   ```bash
   git push origin update-events
   ```

#### Create a Pull Request for Jamie:
1. Go to GitHub and create a PR from `update-events` to `main`.
2. Review the changes and merge the PR into the `main` branch.

---

### 5. **Merge and Resolve Any Conflicts**

#### Merge Conflicts:
- If there are any merge conflicts between the `add-book-reviews` and `update-events` branches, Git will notify you when trying to merge. You will need to manually resolve the conflicts before committing the final merge.
- After resolving the conflicts, run:
   ```bash
   git add <resolved_files>
   git commit -m "Resolved merge conflicts"
   git push origin main
   ```

Once both PRs are merged into the `main` branch, your project will be complete, with a Book Reviews section and an updated Events page.

---

### 6. **Final Verification**

- Check the repository's `main` branch on GitHub to verify that all changes have been merged successfully.
- The live website should now reflect the new Book Reviews section and the updated Events page.

This process simulates a real-world collaborative workflow, where developers contribute to different parts of a project, manage branches, and resolve conflicts.
