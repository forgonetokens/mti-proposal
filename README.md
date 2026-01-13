# Member Technology Initiative — Local 478 Proposal

A reveal.js presentation for proposing member technology tools to the IATSE Local 478 Executive Board.

## Deploying to GitHub Pages

### Option 1: Quick Deploy (Recommended)

1. **Create a new GitHub repository**
   ```bash
   # Initialize git if not already done
   git init
   git add .
   git commit -m "Initial commit: MTI proposal presentation"
   ```

2. **Push to GitHub**
   ```bash
   # Create repo on GitHub first, then:
   git remote add origin https://github.com/YOUR_USERNAME/mti-proposal.git
   git branch -M main
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click **Settings** → **Pages** (in the left sidebar)
   - Under "Source", select **Deploy from a branch**
   - Choose **main** branch and **/ (root)** folder
   - Click **Save**

4. **Access your presentation**
   - Wait 1-2 minutes for deployment
   - Your presentation will be live at: `https://YOUR_USERNAME.github.io/mti-proposal/`

### Option 2: Using GitHub CLI

```bash
# Create and push in one step
gh repo create mti-proposal --public --source=. --remote=origin --push

# Enable Pages
gh api repos/YOUR_USERNAME/mti-proposal/pages -X POST -f source='{"branch":"main","path":"/"}'
```

## Viewing Locally

Just open `index.html` in any modern web browser. No build step or server required.

```bash
# macOS
open index.html

# Linux
xdg-open index.html

# Or use any local server
python -m http.server 8000
# Then visit http://localhost:8000
```

## Presentation Controls

| Action | Control |
|--------|---------|
| Next slide | → or Space |
| Previous slide | ← or Backspace |
| Overview mode | Esc |
| Fullscreen | F |
| Speaker notes | S |

## Contents

**Main Presentation (8 slides)**
1. Title
2. The Opportunity (current pain points)
3. Proposed Solution (6 tools)
4. The Investment (cost comparison)
5. Engagement Model (phased approach)
6. Ownership & Licensing Terms (IP arrangement)
7. The Bigger Picture (ASA opportunity)
8. Next Steps

**Draft Agreement (6 slides)**
- Section 1: Scope of Work
- Section 2: Compensation
- Section 3: Intellectual Property
- Section 4: Project Governance
- Section 5: Disclosure & Conflict of Interest
- Section 6: Signatures

## Customization

The presentation uses CSS custom properties for easy theming:

```css
:root {
  --primary: #1e3a5f;   /* Navy blue */
  --accent: #d4a84b;    /* Gold */
  --secondary: #e8eef4; /* Light blue-gray */
  --muted: #5a6978;     /* Muted text */
}
```

## License

This presentation template is provided for IATSE Local 478 internal use.
