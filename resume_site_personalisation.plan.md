Personalize Academic Pages for fidankarimova.github.io

What this codebase is





Stack: Jekyll static site with the Academic Pages theme (fork of Minimal Mistakes).



Key idea: Site chrome and author sidebar come from [_config.yml](_config.yml). Long-form sections use Markdown under [_pages/](_pages/), [_publications/](_publications/), [_talks/](_talks/), [_teaching/](_teaching/), [_portfolio/](_portfolio/), [_posts/](_posts/). Optional JSON-driven CV lives in [_data/cv.json](_data/cv.json) (used only if you switch the CV nav link to /cv-json/ in [_data/navigation.yml](_data/navigation.yml)).

flowchart LR
  config["_config.yml author + url"]
  about["_pages/about.md home"]
  nav["_data/navigation.yml"]
  cols["_publications _talks etc."]
  config --> Jekyll[Jekyll build]
  about --> Jekyll
  nav --> Jekyll
  cols --> Jekyll
  Jekyll --> GH[GitHub Pages]



Information to send so the site can be updated

Reply with as much as you have; leave items blank if not used (sidebar links hide when empty).

1. GitHub and site URL





GitHub username (must match the site): it is fdnkrmv (your folder name suggests this).



Repository name for user site: must be **fdnkrmv.github.io** (not fdnkrmv.github.io-master).

2. Global branding ([_config.yml](_config.yml))





title: Fidan Karimova.



name: Fidan Karimova



description:  Final-year PhD researcher at The University of Queensland, specialising in AI, machine learning, and spatial-temporal data science. Concurrently serving as a Data Scientist and AI Engineer at Queensland Police Service, delivering production tools and analysis that directly support operational decision-making. Experienced across law enforcement, energy, and academia, with a consistent focus on translating complex data into clear, actionable outcomes for technical and non-technical audiences alike. Equally comfortable building a model, engineering a data pipeline, designing a dashboard, and presenting findings to senior decision-makers. Published at CORE A international venues (ECAI ‘25); work under review at ICML ‘26.



site_theme: light or dark theme with a toggle button.



**repository**: fdnkrmv/fdnkrmv.github.io (owner/repo).

3. Sidebar author block ([_config.yml](_config.yml) → author:)





Profile photo: profile.png under images



name: Fidan Karimova



pronouns She/Her.



bio: PhD Researcher | Academic Instructor



**location, **employer (current org or “Independent” / “PhD student at …”).



**uri**: Personal homepage if different from this GitHub Pages URL.



email: f.karimova@uq.edu.au

Academic / professional links (URLs only for the ones you want shown):





Google Scholar, ORCID, ResearchGate, arXiv, PubMed, Semantic Scholar, etc. (see the author: updated config.yml accordingly

Code / social (usernames or URLs as the template expects):





GitHub username.



LinkedIn. Added username

4. Home page ([_pages/about.md](_pages/about.md))





**title** for the home page (optional override).



Body copy: Replace the long template explainer with your own intro: who you are, what you do, 2–4 short paragraphs, links you care about. You can paste draft text or bullet points.

5. Navigation ([_data/navigation.yml](_data/navigation.yml))





Which top menu items you want visible. Publications, CV, Research, Teaching.



CV format: include the resume.pdf in the cv page

7. Publications ([_publications/*.md](_publications/))

Decision: Remove all sample paper-title-number-* entries.

Here are my publications:
Published
•	Karimova, F., Chen, T., Yang, Y., & Sadiq, S. (2025). Learning a universal crime predictor with knowledge-guided hypernetworks. ECAI 2025. https://doi.org/10.3233/FAIA251027

Under Review
•	Karimova, F., Chen, T., & Sadiq, S. (2026). Knowledge-augmented modelling and retrieval-augmented generation for context-aware urban event prediction. Under review at Information Processing & Management.

In Progress
•	Karimova, F., Chen, T., & Sadiq. S. (2026). Adaptive Learning for Dynamic Urban Environments: Mitigating Temporal Drift and Model Degradation. (Manuscript in preparation)

8. Optional sections





Teaching ([_teaching/](_teaching/)):





BISM1201 - Introduction to Business Information Systems (https://programs-courses.uq.edu.au/course.html?course_code=BISM1201)



BISM2207 - Data Management and Business Intelligence (https://programs-courses.uq.edu.au/course.html?course_code=BISM2207)



BISM7206 - Information Retrieval and Management (https://programs-courses.uq.edu.au/course.html?course_code=BISM7206)



INFS7901 - Data Science and Analytics (https://programs-courses.uq.edu.au/course.html?course_code=INFS7901)



include description of each course below.



My overall responsibilities were:





•     Delivered tutorials across 4 undergraduate and postgraduate courses to 500+ students, consistently translating abstract computational and analytical concepts into practical, applicable skills, receiving strong student feedback.

•     Proactively collaborated with course coordinators on curriculum improvement: proposing, drafting, and iterating on assessments and learning materials aligned with emerging research and industry practice.

•     Mentored students through open-ended, complex data projects from initial concept to working solution, developing structured problem-solving and communication skills essential for geospatial science careers.

•     Experienced teaching in diverse settings including laboratory-based and applied analytics environments, with scope to contribute to field-based and GIS-specific curriculum.

•     Capability to extend teaching into GIS, spatial data science, and GeoAI curriculum, including field-based and applied geospatial learning environments.





Instead of Portfolio, create Research page - a _research/





here we discuss what my research focuses on.



main text explaining my overall research 



then below have these texts written with some relevant image below each title.





Spatial-Temporal Learning



Remote Sensing



Urban Event Forecasting



Large Language Models



Explainable AI









Blog ([_posts/](_posts/)): no  blog; hide from nav and ignore.

9. Downloads





PDFs (CV, papers): filenames and files to place under [files/](files/) 



How to run locally (preview before pushing)

From the repo root on macOS (from [README.md](README.md)):





Install Ruby (e.g. Homebrew), Node, and Bundler: gem install bundler.



bundle config set --local path 'vendor/bundle' (avoids permission issues), then bundle install.



bundle exec jekyll serve -l -H localhost



Open http://localhost:4000 — restart the server after changing [_config.yml](_config.yml).

Alternative: docker compose up if you use Docker (see [README.md](README.md)).



How to get https://fidankarimova.github.io live





Create or use the GitHub account fidankarimova.



Repository name: fidankarimova.github.io (public user site).



Push this project’s contents to the default branch (main or master).



In the repo on GitHub: Settings → Pages → deploy from the same branch, root / (standard Jekyll build). Wait a few minutes for the first build.



Critical: In [_config.yml](_config.yml), set url: https://fidankarimova.github.io and baseurl: "" so links and feeds resolve correctly.

If the repo is new or renamed from fidankarimova.github.io-master, ensure the remote repo name on GitHub is exactly fidankarimova.github.io, not a suffixed name.



After you reply

Once you paste the information above (even in draft form), the next step in Agent mode is to apply edits to [_config.yml](_config.yml), [_pages/about.md](_pages/about.md), [_data/navigation.yml](_data/navigation.yml), CV and collections, add your photo under images/, and remove or replace sample publications — without changing theme machinery unnecessarily.