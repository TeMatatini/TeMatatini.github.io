<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Royal Edinburgh Military Tattoo 2026</title>

  <style>
    :root {
      --bg: #0f0f0f;
      --card: #1a1a1a;
      --hover: #222;
      --text: #f5f5f5;
      --muted: #aaa;
      --accent: #c9a24d;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      min-height: 100vh;
      background: radial-gradient(circle at top, #181818, var(--bg));
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
      color: var(--text);
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 24px;
    }

    .container {
      max-width: 900px;
      width: 100%;
      text-align: center;
    }

    h1 {
      font-size: clamp(2rem, 4vw, 2.8rem);
      margin-bottom: 12px;
      letter-spacing: 0.03em;
    }

    p {
      color: var(--muted);
      margin-bottom: 40px;
      font-size: 1.05rem;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 24px;
    }

    a.card {
      text-decoration: none;
      background: linear-gradient(180deg, var(--card), #111);
      border-radius: 18px;
      padding: 36px 28px;
      color: var(--text);
      transition: transform 0.25s ease, box-shadow 0.25s ease, background 0.25s ease;
      box-shadow: 0 10px 30px rgba(0,0,0,0.4);
      position: relative;
      overflow: hidden;
    }

    a.card::after {
      content: "";
      position: absolute;
      inset: 0;
      background: linear-gradient(120deg, transparent, rgba(255,255,255,0.05), transparent);
      opacity: 0;
      transition: opacity 0.25s ease;
    }

    a.card:hover {
      transform: translateY(-6px);
      background: linear-gradient(180deg, var(--hover), #111);
      box-shadow: 0 18px 40px rgba(0,0,0,0.55);
    }

    a.card:hover::after {
      opacity: 1;
    }

    .location {
      font-size: 1.6rem;
      font-weight: 600;
      margin-bottom: 8px;
      letter-spacing: 0.04em;
    }

    .studio {
      color: var(--accent);
      font-size: 0.95rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
    }

    footer {
      margin-top: 40px;
      font-size: 0.85rem;
      color: #777;
    }
  </style>
</head>
<body>

  <div class="container">
    <h1>Royal Edinburgh Military Tattoo 2026</h1>
    <p>Select your event location</p>

    <div class="grid">
      <a class="card" href="https://www.edintattooauckland.co.nz">
        <div class="location">Auckland</div>
        <div class="studio">New Zealand</div>
      </a>

      <a class="card" href="https://www.edintattoobrisbane.com.au">
        <div class="location">Brisbane</div>
        <div class="studio">Australia</div>
      </a>
    </div>

    <footer>
      © Te Matatini Society Inc, 2026
    </footer>
  </div>

</body>
</html>
