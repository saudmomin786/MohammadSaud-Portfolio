# Portfolio Website Build - Prompts

---

## Prompt 1: Generate PRD

Attach your resume and a Dribbble screenshot of a design you like. Use any LLM.

```
I'm a data analyst building a personal portfolio website. I'm attaching my resume and a screenshot of a design I like from Dribbble.

Based on my resume and the attached design, generate a PRD for my portfolio website.

The PRD should include:

1. SITE SECTIONS (list each section with a one-liner on what goes in it)
   Must include: Hero, About, Skills, Projects, Live Dashboards (for Tableau/Power BI embeds), Experience, Education, Contact

2. PROJECT CARDS (for each project from my resume)
   - Title
   - One-line description
   - Tools used
   - One key metric or finding
   - What visual to show (dashboard embed, chart screenshot, etc.)

3. COPY (write the actual text for each section based on my resume, first person, conversational but professional. No lorem ipsum.)

4. DESIGN DIRECTION (based on the attached Dribbble screenshot, describe the visual style in 4-5 bullet points covering: color palette, typography feel, layout style, spacing, and overall mood)

Keep the PRD to 2-3 pages max. No filler. Just the structure, the content, and the visual direction.
```

---

## Prompt 2: Lovable Build

Upload your PRD, your resume, and the same Dribbble screenshot to Lovable.

```
Build me a personal portfolio website for a data analyst.

I'm attaching:
1. My PRD (follow this for structure, content, and design direction)
2. My resume (use this for all personal details, experience, and projects)
3. A Dribbble screenshot (match this visual style as closely as possible)

Additional build notes:
- Single page app with smooth scroll navigation
- Dark mode as default with a light mode toggle
- Sticky minimal nav at the top
- Subtle scroll animations (nothing over the top)
- Project cards that show the title, tools, and key metric at a glance
- A dedicated "Live Dashboards" section with 2-3 responsive iframe containers. Use placeholder iframes for now with a comment saying "Replace with Tableau Public or Power BI embed URL"
- Contact section with a simple form or direct email link
- Make it responsive for mobile

Keep it clean. Professional but not boring.
```

---

## Prompt 3: Dashboard Integration

Use this in Lovable after your site is built to replace the placeholder iframes with real dashboards.

```
Update the Live Dashboards section to embed real dashboards.

Dashboard 1 - Tableau:
Replace the first placeholder iframe with a Tableau Public embed.
The embed URL is: [PASTE YOUR TABLEAU PUBLIC EMBED URL HERE]
Use this iframe format: src should append "?:embed=y&:display_count=no&:showVizHome=no" to the URL. Set width to 100% and height to 600px.

Dashboard 2 - Power BI:
Replace the second placeholder iframe with a Power BI embed.
The embed URL is: [PASTE YOUR POWER BI PUBLISH-TO-WEB URL HERE]
Set width to 100% and height to 600px.

Also:
- Add a loading skeleton for each dashboard while the iframe loads
- Add a caption below each embed with the dashboard title and one-line description
- On mobile, swap the iframe for a screenshot/thumbnail with a note saying "View on desktop for the interactive version"
- Keep spacing clean, wrap each embed in a card container
```
