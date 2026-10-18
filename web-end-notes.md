<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Web Page Endnotes</title>
  <style>
    /* 1. Global Setup & Fixed Header Prevention */
    html {
      scroll-behavior: smooth;
      /* Adjust this value if you have a sticky top nav bar (e.g., 60px) */
      scroll-padding-top: 24px; 
    }

    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
      line-height: 1.6;
      max-width: 680px;
      margin: 40px auto;
      padding: 0 20px;
      color: #333;
    }

    /* 2. In-text Citation Links */
    .citation-ref {
      font-size: 0.75em;
      vertical-align: super;
      line-height: 0;
    }

    .citation-link {
      text-decoration: none;
      color: #0056b3;
      padding: 0 2px;
      border-radius: 3px;
      transition: background-color 0.2s ease;
    }

    .citation-link:hover,
    .citation-link:focus {
      background-color: #e6f2ff;
      text-decoration: underline;
    }

    /* 3. Endnotes Section Layout */
    .endnotes-section {
      margin-top: 80px;
      border-top: 1px solid #eaeaea;
      padding-top: 24px;
      font-size: 0.9rem;
      color: #555;
    }

    .endnotes-title {
      font-size: 1.2rem;
      margin-bottom: 20px;
      color: #111;
    }

    .endnotes-list {
      padding-left: 20px;
    }

    .endnotes-list li {
      margin-bottom: 12px;
      padding: 4px 8px;
      border-radius: 4px;
      transition: background-color 0.5s ease;
    }

    /* 4. Active Target Highlight Animation */
    .endnotes-list li:target {
      background-color: #e6f2ff;
      /* Keeps the item highlighted; will fade back if you navigate away */
      transition: background-color 0.1s ease; 
    }

    .back-link {
      text-decoration: none;
      color: #0056b3;
      margin-left: 6px;
      display: inline-block;
    }

    .back-link:hover,
    .back-link:focus {
      transform: translateY(-1px);
    }
  </style>
</head>
<body>

  <main>
    <article>
      <h1>Understanding Web Standards</h1>
      <p>
        Building accessible interfaces requires a strict dedication to using semantic HTML tags whenever possible<span class="citation-ref"><a href="#note-1" id="ref-1" class="citation-link" aria-label="Footnote 1">1</a></span>. 
        When developers rely on native browser behaviors, complex components require substantially less custom JavaScript overhead to achieve accessibility goals across major devices<span class="citation-ref"><a href="#note-2" id="ref-2" class="citation-link" aria-label="Footnote 2">2</a></span>.
      </p>
    </article>
  </main>

  <!-- Endnotes -->
  <footer class="endnotes-section" aria-label="Endnotes">
    <h2 class="endnotes-title" id="endnotes-heading">Notes</h2>
    <ol class="endnotes-list" aria-labelledby="endnotes-heading">
      <li id="note-1">
        Smith, A. (2026). <em>The Semantic Web and Accessibility</em>. W3C Publishing.
        <a href="#ref-1" class="back-link" aria-label="Back to content reference 1">↩</a>
      </li>
      <li id="note-2">
        Doe, B. (2025). <em>Native Browser Mechanics</em>. Digital Press.
        <a href="#ref-2" class="back-link" aria-label="Back to content reference 2">↩</a>
      </li>
    </ol>
  </footer>

</body>
</html>
