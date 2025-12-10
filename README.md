Jekyll build trigger at [Current time is Tuesday, December 9, 2025 at 5:09:53 PM MST.]

# Clean Futuristic Project Template (starter)

What this provides
- Minimal index.html with a grid of project cards
- styles.css implements dark+light themes, geometric typography, asymmetrical grid, hover/glitch effects, and accessibility defaults

How to use
1. Copy `index.html` and `styles.css` to your repo root (or adapt into your templating engine).
2. Replace example project-card blocks with real project entries. Each project should:
   - Have a thumbnail at `assets/<project>-thumb.webp`
   - Link to `projects/<project>.html` (create a simple project file using the same header/footer)
3. Optimize thumbnails: use WebP, set width/height attributes, and use loading="lazy".
4. Test responsiveness and keyboard-only navigation.

Suggested project page skeleton (projects/project-1.html)

```html
<!doctype html><html lang="en"><head>...same head...</head><body>
  <main class="container">
    <article class="project-detail">
      <h1>Project One</h1>
      <p>One-sentence summary</p>
      <!-- add screens, writeup, links, repo, tech list -->
    </article>
  </main>
</body></html>
```

Performance & accessibility notes
- Use <img width height> and srcset for responsive images to avoid layout shifts.
- Add aria-labels where necessary and ensure focusable elements are visible.
- Consider preloading your primary font (link rel=preload) for visual stability.
- Respect prefers-reduced-motion for animations.

Deployment notes
- This works on GitHub Pages. If you previously used a CNAME and want to remove the custom domain, delete the `CNAME` file and update the Pages settings in the repo.
- If you'd like, I can push these files to a branch and open a PR for you—say "please add these files" to proceed.

If you want, I can:
- Convert this into Jekyll includes/layouts (if you use Jekyll).
- Create a script to auto-generate project cards from a projects/ directory or JSON.
- Add a light/dark toggle UI and small JS to animate it smoothly.

Which of those would you like next?
