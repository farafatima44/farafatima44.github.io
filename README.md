# Fara Fatima — Java Full Stack Developer Portfolio

Personal portfolio showcasing my experience building and modernizing **full-stack enterprise applications** using Java, Spring Boot, React, Angular, REST APIs, microservices, and cloud technologies.

I have **8+ years of software development experience** across financial services, healthcare, and enterprise applications, with a focus on building scalable backend services, responsive web applications, APIs, and cloud-based solutions.

## Core Technologies

* **Backend:** Java, Spring Boot, Spring MVC, Spring Security, Spring Data JPA, REST APIs, Microservices
* **Frontend:** React, Angular, JavaScript, TypeScript, HTML, CSS, RxJS, Redux
* **Cloud & DevOps:** AWS, Docker, Kubernetes, Jenkins, GitHub Actions, Terraform
* **Messaging & Integration:** Kafka, AWS SNS, AWS SQS, GraphQL
* **Databases:** PostgreSQL, Oracle, MySQL, DynamoDB, Redis, Elasticsearch
* **Testing:** JUnit, Mockito, REST API testing, integration testing
* **AI & Developer Tools:** OpenAI API, LangChain, GitHub Copilot, Cursor, Claude Code

## Portfolio Highlights

The portfolio includes:

* Professional experience and project history
* Full-stack application development
* Java and Spring Boot microservices
* React and Angular frontend development
* REST API and backend development
* AWS cloud and containerized applications
* Kafka-based event-driven systems
* AI-assisted application development
* Selected technical projects
* Resume and professional contact information

## What's Interactive

* Animated portfolio background and cursor effects
* Typed headline highlighting different areas of expertise
* Scroll progress indicator
* Active section navigation
* Animated experience statistics
* Interactive project cards
* Keyboard-navigable experience tabs
* Filterable technical skills
* Dark/light mode with saved preference
* Responsive mobile navigation
* Copy-email button with confirmation
* Reduced-motion support for accessibility

## Files

```text
index.html    Main portfolio page
resume.pdf    Optional resume linked from the portfolio
README.md     Project documentation
```

## Hosting on GitHub Pages

### 1. Create the repository

Create a GitHub repository using your GitHub username:

```text
YOUR-USERNAME.github.io
```

The repository must be public for the standard GitHub Pages setup.

### 2. Push the files

```bash
cd portfolio
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-USERNAME.github.io.git
git push -u origin main
```

### 3. Enable GitHub Pages

In the repository:

**Settings → Pages → Build and deployment**

Select:

* **Source:** Deploy from a branch
* **Branch:** main
* **Folder:** / (root)

Then click **Save**.

### 4. Open the portfolio

After GitHub Pages finishes deploying, the portfolio will be available at:

```text
https://YOUR-USERNAME.github.io
```

Future changes will automatically deploy when you push them to the `main` branch.

## Adding Your Resume

The **Resume** button links to:

```text
resume.pdf
```

Place your resume PDF in the root of the repository using that exact filename:

```text
portfolio/
├── index.html
├── resume.pdf
└── README.md
```

Then commit and push the change:

```bash
git add .
git commit -m "Add resume"
git push
```

## Custom Domain

You can connect a custom domain through:

**GitHub → Repository → Settings → Pages → Custom domain**

After configuring your domain's DNS records, enable **Enforce HTTPS** once the certificate is available.

## Editing the Portfolio

The portfolio is intentionally simple and lightweight.

Everything is contained in:

```text
index.html
```

The page does not require a build process or frontend framework.

The main styling variables are defined near the beginning of the `<style>` section:

```css
--accent: #1F6F5C;
--ink: #0D1B2A;
```

You can update these values to change the primary visual theme.

## Technical Notes

* Single self-contained HTML file
* No build step
* No JavaScript framework dependency
* Responsive design
* Keyboard-accessible navigation
* Visible keyboard focus states
* Dark/light theme support
* `localStorage` used for theme preference
* `prefers-reduced-motion` support
* Google Fonts loaded externally
* Works offline with the exception of externally loaded fonts

## Contact

For professional opportunities, collaboration, or technical discussions:

**Fara Fatima**
Java Full Stack Developer
Email: `faraftima8@gmail.com`

---

Built with HTML, CSS, and JavaScript.
