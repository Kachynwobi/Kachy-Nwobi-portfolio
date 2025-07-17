<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>{{ page.title }}</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet" />
  <style>
    :root {
      --bg-light: #f9f9f9;
      --bg-dark: #121212;
      --text-light: #333;
      --text-dark: #f0f0f0;
      --accent: #004d99;
      --link-hover: #007acc;
    }
    body {
      font-family: 'Inter', sans-serif;
      margin: 0;
      padding: 0;
      background-color: var(--bg-light);
      color: var(--text-light);
      transition: background 0.3s, color 0.3s;
    }
    body.dark-mode {
      background-color: var(--bg-dark);
      color: var(--text-dark);
    }
    a {
      color: var(--accent);
      text-decoration: none;
    }
    a:hover {
      color: var(--link-hover);
    }
    header {
      background: var(--accent);
      color: white;
      padding: 2rem 1rem;
      text-align: center;
    }
    nav {
      background: #ffffff;
      display: flex;
      justify-content: center;
      gap: 2rem;
      padding: 1rem;
      border-bottom: 1px solid #ddd;
    }
    nav a {
      font-weight: 600;
    }
    body.dark-mode nav {
      background: #1e1e1e;
    }
    nav a:hover {
      color: var(--accent);
    }
    .toggle-dark {
      position: fixed;
      top: 1rem;
      right: 1rem;
      background: #ccc;
      padding: 0.5rem 1rem;
      border: none;
      border-radius: 20px;
      cursor: pointer;
      font-weight: bold;
    }
    section {
  max-width: 900px;
  margin: 2rem auto;
  padding: 2rem 1rem;
  border-radius: 12px;
  background-color: #ffffff;
  transition: background-color 0.3s;
}
    h2 {
      color: var(--accent);
      border-bottom: 2px solid #eee;
      padding-bottom: 0.5rem;
    }
    .skills table {
      width: 100%;
      border-collapse: collapse;
    }
    .skills td {
      padding: 0.5rem;
      border: 1px solid #ddd;
    }
    .project img {
      width: 100%;
      max-width: 700px;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      margin: 1rem 0;
    }
    .contact a {
      display: inline-block;
      margin: 0.5rem;
      padding: 0.5rem 1rem;
      background: #e0f0ff;
      border-radius: 5px;
      text-decoration: none;
      color: var(--accent);
      font-weight: 600;
    }
    footer {
      text-align: center;
      padding: 1rem;
      background: #eee;
      font-size: 0.9rem;
      margin-top: 4rem;
    }
    body.dark-mode footer {
  background: #1e1e1e;
}

body.dark-mode section {
  background-color: #1e1e1e;
}
  </style>
</head>
<body>
  <button class="toggle-dark" onclick="document.body.classList.toggle('dark-mode')">🌓 Theme</button>

  <header>
    <h1>Kachy Nwobi</h1>
    <p>Geospatial Data Engineer | AEC & Urban Resilience | Data-Driven Storytelling</p>
  </header>

  <nav>
    <a href="#about">About</a>
    <a href="#skills">Skills</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="about">
    <h2>About Me</h2>
    <p>I’m a geospatial data engineer with 5+ years of experience curating, transforming, and deploying spatial datasets to power intelligent decision-making across AEC, climate, and urban resilience domains.</p>
  </section>

  <section id="skills" class="skills">
    <h2>Core Skills</h2>
    <table>
      <tr><td><strong>GIS Tools</strong></td><td>ArcGIS Pro, ArcGIS Online, ArcGIS Enterprise, QGIS, CityEngine</td></tr>
      <tr><td><strong>Data Tools</strong></td><td>GDAL, Python, SQL, GeoTIFF, GeoJSON, LAS/LAZ</td></tr>
      <tr><td><strong>AEC Platforms</strong></td><td>ArcGIS GeoBIM, Autodesk Forma, Revit, Civil 3D</td></tr>
      <tr><td><strong>Visualization</strong></td><td>Web maps, dashboards, 3D terrain</td></tr>
      <tr><td><strong>Collaboration</strong></td><td>GitHub, Jira, Figma</td></tr>
    </table>
  </section>

  <section id="projects">
    <h2>Featured Projects</h2>

    <div class="project">
      <h3>ArcGIS GeoBIM: Connecting GIS + BIM</h3>
      <p>Integrated BIM models with GIS features for 3D infrastructure coordination.</p>
      <img src="image/arcgis-geobim.png" alt="ArcGIS GeoBIM">
      <p><a href="https://www.esri.com/en-us/arcgis/products/arcgis-geobim/overview">Learn more</a></p>
    </div>

    <div class="project">
      <h3>ArcGIS for Autodesk Forma</h3>
      <p>Real-time GIS integration to support collaborative urban design workflows.</p>
      <img src="image/arcgisforautodeskforma.png" alt="ArcGIS for Autodesk Forma">
      <p><a href="https://www.esri.com/en-us/arcgis/products/arcgis-for-autodesk-forma/overview">Learn more</a></p>
    </div>

    <div class="project">
      <h3>PolicyMap: Mapping Vulnerability</h3>
      <p>Developed thematic maps for flood vulnerability and public infrastructure analysis.</p>
      <img src="image/policymap_project.png" alt="PolicyMap Midwest Floods">
      <p><a href="https://policymap.wpengine.com/blog/the-midwest-floods-and-socially-vulnerable-populations">Read the article</a></p>
    </div>
  </section>

  <section id="contact" class="contact">
    <h2>Connect With Me</h2>
    <a href="mailto:kachynwobi@gmail.com">Email</a>
    <a href="https://www.linkedin.com/in/kachy-nwobi-3463b64a/">LinkedIn</a>
    <a href="https://github.com/Kachynwobi/kachynwobi_portfolio/blob/7b2df8c69f2e50f516893cb96101ef6bee4d34a6/image/Kachy_Nwobi_Resume_GDE.pdf">Resume</a>
  </section>

  <footer>
    <p>© 2025 Kachy Nwobi · Powered by GitHub Pages</p>
  </footer>
</body>
</html>
