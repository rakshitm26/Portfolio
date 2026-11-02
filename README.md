# 🚀 Rakshit Malik's Portfolio & Learning Hub

A modern, high-performance personal portfolio built exclusively with **semantic HTML5** and **modern CSS3**. Designed with clean markup, inline edit markers, and CSS design tokens so you can update and customize it anytime with zero build tools or complex dependencies.

---

## 📂 Project Structure

```text
S&AI(AI Topic)/
├── index.html       # Semantic HTML5 page with explicit edit markers (✏️)
├── styles.css       # Dark & Sleek Tech CSS with custom variables and animations
└── README.md        # Complete editing guide, deployment steps, & learning masterplan
```

---

## ⚡ Quick Start: Viewing Your Portfolio

1. **Directly in Browser**: Double-click [`index.html`](file:///Users/rakshitmalik/Desktop/S&AI(AI Topic)/index.html) to open it in Chrome, Safari, or Arc.
2. **In VS Code or Cursor**:
   - Right-click `index.html` and select **"Open with Live Server"** (if the Live Server extension is installed).
   - Alternatively, open the terminal and run:
     ```bash
     python3 -m http.server 3000
     ```
     Then open `http://localhost:3000` in your browser.

---

## ✏️ How to Edit Your Portfolio

Every section in [`index.html`](file:///Users/rakshitmalik/Desktop/S&AI(AI Topic)/index.html) is labeled with `<!-- ✏️ EDIT HERE: ... -->` comments so you know exactly where to make updates.

### 1. Update Your Name, Bio, and Social Handles
- Open [`index.html`](file:///Users/rakshitmalik/Desktop/S&AI(AI Topic)/index.html).
- Press `Ctrl + F` or `Cmd + F` and search for `Rakshit Malik` or `EDIT HERE`.
- Replace the bio text, headlines, and social links (`https://github.com`, `https://linkedin.com`, `rakshit@example.com`) with your real profiles.

### 2. Configure Your Cal.com Booking Widget
- In `index.html`, locate the `#booking` section:
  ```html
  <iframe 
    src="https://cal.com/YOUR_USERNAME?embed=true" 
    frameborder="0" 
    class="cal-iframe"
    title="Schedule an Appointment via Cal.com"
    loading="lazy">
  </iframe>
  ```
- Replace `rakshitmalik` with your actual Cal.com username (e.g. `https://cal.com/john-doe` or `https://cal.com/john-doe/15min`).

### 3. Adding a New Project Card
To add a new project, copy and paste this snippet inside `<div class="projects-grid">`:

```html
<article class="project-card">
  <div class="project-header">
    <div class="project-folder-icon">
      <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 19a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h5l2 3h9a2 2 0 0 1 2 2z"/></svg>
    </div>
    <div class="project-links">
      <a href="https://github.com/your-username/repo" target="_blank" rel="noopener noreferrer" title="View Code">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"/></svg>
      </a>
      <a href="https://your-demo-url.vercel.app" target="_blank" rel="noopener noreferrer" title="Live Preview">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"/><polyline points="15 3 21 3 21 9"/><line x1="10" y1="14" x2="21" y2="3"/></svg>
      </a>
    </div>
  </div>
  <h3 class="project-title">Your Project Name</h3>
  <p class="project-description">
    Describe what problem your project solves, how it works, and what technologies you used.
  </p>
  <div class="project-tags">
    <span>Python</span>
    <span>Vercel</span>
    <span>AI</span>
  </div>
</article>
```

### 4. Customizing Theme Colors & Styles
Open [`styles.css`](file:///Users/rakshitmalik/Desktop/S&AI(AI Topic)/styles.css) and look at the top `:root` block:
```css
:root {
  --bg-primary: #07090e;      /* Main background */
  --accent-cyan: #38bdf8;     /* Cyan accent color */
  --accent-indigo: #6366f1;   /* Indigo accent */
  --text-primary: #f8fafc;    /* Heading text */
}
```
Change any hex color code, and the entire website will immediately reflect your new palette.

---

## 🌐 Deploying Your Portfolio in 2 Minutes (Free)

### Method A: Deploy with Vercel (Recommended)
1. Push this folder to a GitHub repository.
2. Visit [vercel.com](https://vercel.com) and click **"Add New Project"**.
3. Import your GitHub repository.
4. Click **"Deploy"**! Vercel will instantly publish your site with an SSL certificate and custom domain support.

### Method B: Deploy with GitHub Pages
1. In your GitHub repository, go to **Settings > Pages**.
2. Under **Build and deployment > Branch**, select `main` and `/ (root)`.
3. Click **Save**. Your site will be live at `https://<your-username>.github.io/<repo-name>/`.

---

## 📚 Master Learning Roadmap

A structured guide for the skills you are pursuing:

### 1. Python Mastery
- **Phase 1: Fundamentals**: Variables, conditionals, loops, functions, lists, dictionaries.
- **Phase 2: Terminal Scripting**: Writing CLI scripts using `sys.argv`, `argparse`, and file I/O (`open()`, `csv`, `json`).
- **Phase 3: Python for Finance & Data**: Working with `pandas`, `numpy`, and fetching live stock/crypto data via APIs (`yfinance`, `alpha_vantage`).

### 2. AI Tools & Rapid Interactive Prototyping
- **Cursor**:
  - Use `Cmd + K` for in-line edits and `Cmd + L` (Chat) to ask architectural questions.
  - Create `.cursorrules` files in your projects to guide AI code generation style.
- **Genspark**:
  - Use Genspark Sparkpages and agentic search for deep-dive research into financial models, software frameworks, and competitor analysis.
- **Motion Sites & CSS Animations**:
  - Master CSS `@keyframes`, transitions, and layout transformations (`scale`, `translate`).
  - Study interactive micro-interactions on modern landing pages (Framer, Linear design principles).
- **Wondershare Filmora**:
  - Record project screen recordings, add dynamic camera zooms, text overlays, and sound design to create 60-second video showcases for Twitter and LinkedIn.
- **Cal.com**:
  - Set up bookable meeting types (e.g. 15-min Coffee Chat, 30-min Project Collab) and embed them into your web pages.

### 3. Developer Fundamentals
- **CLI (Command Line)**:
  - Essential commands: `ls -la`, `cd`, `mkdir`, `rm -rf`, `touch`, `cat`, `grep`, `curl`.
  - Managing environments: `python3 -m venv .venv` and `source .venv/bin/activate`.
- **VS Code**:
  - Top extensions: Prettier, Live Server, Python (Microsoft), GitLens, Error Lens.
  - Shortcut mastery: `Cmd + P` (Quick Open), `Cmd + Shift + P` (Command Palette), `Cmd + D` (Multi-select).
- **Git & GitHub**:
  - Daily commands:
    ```bash
    git init
    git add .
    git commit -m "feat: update portfolio hero and projects"
    git branch -M main
    git remote add origin https://github.com/<user>/<repo>.git
    git push -u origin main
    ```

### 4. WorldQuant BRAIN Alpha Modeling & Quantitative Finance
- **WorldQuant BRAIN Alpha Formulation**:
  - **Data Feeds**: Price-volume datasets, corporate fundamental ratios, analyst consensus, and alternative sentiment data.
  - **Mathematical Operators**: Time-series ranking (`ts_rank`), linear decay (`decay_linear`), cross-sectional normalization (`rank`, `zscore`), and group neutralization (`group_neutralize`).
  - **Simulation & Quality Metrics**:
    - **Information Ratio (IR) / Sharpe Ratio**: Target > 1.25 for consistent risk-adjusted returns.
    - **Turnover**: Kept within feasible transaction limits (typically 1% - 70%).
    - **Fitness & Drawdown**: Maximizing fitness score (> 1.0) while minimizing peak-to-trough drawdowns.
    - **Correlation**: Keeping alpha correlations low (< 0.7) relative to the BRAIN alpha pool.
- **Finance Fundamentals**: Income statement, Balance sheet, Cash flow statement, EBITDA, DCF (Discounted Cash Flow).
- **Markets**: Global equities, market microstructure, interest rates, macro indicators (Inflation, Fed policy).
- **Practical Fusion**: Write Python scripts that analyze alpha performance, simulate portfolio rebalancing, and compute Sharpe/Sortino ratios.

# Portfolio
