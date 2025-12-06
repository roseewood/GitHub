<h1 style="font-size: 2.5rem; color:#2c3e50;">🚀 Learn GitHub</h1>

<p>Welcome to the <strong>ultimate GitHub learning guide</strong>.<br>
This README is designed so that <strong>anyone can learn Git + GitHub from zero to advanced</strong>, simply by reading it.</p>

<ul>
  <li>Clear explanations</li>
  <li>Examples</li>
  <li>Diagrams</li>
  <li>Tables</li>
  <li>Best practices</li>
  <li>Advanced concepts</li>
  <li>Real workflows</li>
</ul>

<hr>

<h1>📘 What Are Git & GitHub?</h1>

<h2>🔧 What is Git?</h2>

<p>
Git is a <strong>distributed version control system</strong> (VCS).  
It helps developers:
</p>

<ul>
  <li>Track changes in code</li>
  <li>Restore previous versions</li>
  <li>Work on features safely</li>
  <li>Collaborate without overwriting code</li>
</ul>

<p><em>Think of Git as a <strong>time-machine + teamwork tool</strong> for code.</em></p>

<h2>💻 What is GitHub?</h2>

<p>GitHub is an online platform built on top of Git. It provides:</p>

<ul>
  <li>Cloud hosting for repositories</li>
  <li>Collaboration tools</li>
  <li>Automation (CI/CD)</li>
  <li>Project management</li>
  <li>Documentation hosting</li>
</ul>

<blockquote>
  Git = Version control <br>
  GitHub = Social network + cloud for Git projects
</blockquote>

<hr>

<h1>🛠 Installing & Configuring Git</h1>

<h2> Step 1: Install Git</h2>

<p>Download Git from:  
<a href="https://git-scm.com/downloads">https://git-scm.com/downloads</a></p>

<pre>
git --version
</pre>

<h2> Step 2: Configure Git (Required)</h2>

<pre>
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
</pre>

<hr>

<h1>📁 Repositories — Local & Remote</h1>

<p>A <strong>repository (repo)</strong> is a folder tracked by Git.</p>

<p>Two types:</p>
<ul>
  <li><strong>Local repository</strong> (on your computer)</li>
  <li><strong>Remote repository</strong> (on GitHub)</li>
</ul>

<h2> Create a Local Repository</h2>

<pre>
mkdir my-project
cd my-project
git init
</pre>

<h2> Create a Remote Repository (GitHub)</h2>

<ol>
  <li>Log in → Click <strong>New Repository</strong></li>
  <li>Enter a name</li>
  <li>Click <strong>Create</strong></li>
</ol>

<h2> Link Local → GitHub</h2>

<pre>
git remote add origin https://github.com/username/repo.git
git push -u origin main
</pre>

<hr>

<h1>📄 Understanding Git Workflow</h1>

<h3>Diagram: Local → GitHub Workflow</h3>

<pre>
A[Working Directory] → git add → Staging Area → git commit → Local Repo → git push → GitHub Remote Repo
</pre>

<hr>

<h1>🧱 Essential Git Commands</h1>

<table>
  <tr>
    <th>Command</th>
    <th>Purpose</th>
  </tr>
  <tr><td>git init</td><td>Start a new repo</td></tr>
  <tr><td>git clone</td><td>Copy a GitHub repo</td></tr>
  <tr><td>git add</td><td>Stage changes</td></tr>
  <tr><td>git commit</td><td>Save changes</td></tr>
  <tr><td>git status</td><td>Show file states</td></tr>
  <tr><td>git push</td><td>Upload to GitHub</td></tr>
  <tr><td>git pull</td><td>Download from GitHub</td></tr>
  <tr><td>git log</td><td>Show commit history</td></tr>
</table>

<hr>

<h1>🔁 Commit, Push & Pull (Core Git Flow)</h1>

<pre>
git add .
git commit -m "Describe what you changed"
git push origin main
git pull origin main
</pre>

<hr>

<h1>🌿 Branching — Safe Way to Build Features</h1>

<h3>Create a branch</h3>
<pre>git checkout -b login-feature</pre>

<h3>Switch branches</h3>
<pre>git checkout main</pre>

<h3>Merge branch</h3>
<pre>git merge login-feature</pre>

<h3>Delete branch</h3>
<pre>git branch -d login-feature</pre>

<hr>

<h1>📥 Pull Requests (PRs) — Collaboration Workflow</h1>

<p>Pull Requests allow:</p>

<ul>
  <li>Reviewing code</li>
  <li>Discussing changes</li>
  <li>Running automated tests</li>
  <li>Merging feature branches</li>
</ul>

<ol>
  <li>Push your branch</li>
  <li>Go to <strong>Pull Requests</strong></li>
  <li>Click <strong>New Pull Request</strong></li>
  <li>Write title & description</li>
  <li>Add reviewers</li>
  <li>Submit</li>
</ol>

<hr>

<h1>🤝 Collaboration — Forks & Clones</h1>

<h2>Clone a repo</h2>
<pre>
git clone https://github.com/user/repo.git
</pre>

<h2>Forking</h2>
<p>Fork = Copy someone’s repo into your GitHub</p>

<h3>Add upstream (original repo)</h3>
<pre>
git remote add upstream https://github.com/original/repo.git
</pre>

<h3>Sync fork</h3>
<pre>
git fetch upstream
git merge upstream/main
</pre>

<hr>

<h1>💼 Issues, Labels, & Milestones</h1>

<h2>Issues Used For</h2>
<ul>
  <li>Bugs 🐞</li>
  <li>Feature requests ✨</li>
  <li>Questions ❓</li>
  <li>Tasks 📌</li>
</ul>

<h2>Labels</h2>

<table>
  <tr><th>Label</th><th>Meaning</th></tr>
  <tr><td>bug</td><td>Something not working</td></tr>
  <tr><td>enhancement</td><td>New feature</td></tr>
  <tr><td>documentation</td><td>Docs needed</td></tr>
  <tr><td>good-first-issue</td><td>Beginner friendly</td></tr>
</table>

<hr>

<h1>🧪 GitHub Actions — Automation & CI/CD</h1>

<h3>Example Workflow</h3>

<pre>
name: CI
on: [push]

jobs:
 build:
  runs-on: ubuntu-latest
  steps:
   - uses: actions/checkout@v2
   - name: Install Packages
     run: npm install
   - name: Run Tests
     run: npm test
</pre>

<hr>

<h1>🌐 GitHub Pages — FREE Website Hosting</h1>

<ol>
  <li>Go to <strong>Settings → Pages</strong></li>
  <li>Select a branch</li>
  <li>Save</li>
</ol>

<p>Your website will appear at:</p>

<p><code>https://username.github.io/repository-name</code></p>

<hr>

<h1>🧠 Advanced Git Concepts</h1>

<h2> Soft Reset (keep changes)</h2>
<pre>git reset --soft HEAD~1</pre>

<h2> Hard Reset (delete changes)</h2>
<pre>git reset --hard HEAD~1</pre>

<h2> Stash (temporary save)</h2>
<pre>
git stash
git stash list
git stash pop
</pre>

<h2> Rebase</h2>
<pre>git rebase main</pre>

<h2> Cherry-pick</h2>
<pre>git cherry-pick &lt;commit-id&gt;</pre>

<h2> Tags</h2>
<pre>
git tag v1.0.0
git push origin v1.0.0
</pre>

<hr>

<h1>🚨 Best Practices Every Developer Should Follow</h1>

<ul>
  <li>Commit small & frequently</li>
  <li>Write meaningful commit messages</li>
  <li>Use branches for each feature</li>
  <li>Use PRs & request reviews</li>
  <li>Keep <code>main</code> always stable</li>
  <li>Automate tests with GitHub Actions</li>
  <li>Document everything</li>
</ul>

<hr>

<h1>📚 Useful Resources</h1>

<ul>
  <li><a href="https://git-scm.com/doc">Git Documentation</a></li>
  <li><a href="https://docs.github.com">GitHub Docs</a></li>
  <li><a href="https://docs.github.com/en/actions">GitHub Actions Docs</a></li>
  <li><a href="https://docs.github.com/en/pages">GitHub Pages Docs</a></li>
</ul>

<hr><br>




<p><strong>Happy Coding! ✨👨‍💻👩‍💻</strong></p>
