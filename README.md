<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <title>HYFY Labs — Coming Soon</title>

  <meta
    name="description"
    content="HYFY Labs — How You Find Yours."
  />

  <style>
    :root {
      --bg: #070a14;
      --text: #f7f8ff;
      --muted: #a8b0c7;
      --cyan: #49f4ff;
      --violet: #b75cff;
      --line: rgba(255,255,255,.12);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      min-height: 100vh;
      font-family:
        Inter,
        system-ui,
        -apple-system,
        BlinkMacSystemFont,
        "Segoe UI",
        sans-serif;

      color: var(--text);

      background:
        radial-gradient(circle at 20% 25%, rgba(73,244,255,.18), transparent 28%),
        radial-gradient(circle at 80% 35%, rgba(183,92,255,.24), transparent 30%),
        linear-gradient(180deg, #080b16 0%, #03050b 100%);

      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
    }

    body::before {
      content: "";
      position: fixed;
      inset: 0;

      background-image:
        linear-gradient(var(--line) 1px, transparent 1px),
        linear-gradient(90deg, var(--line) 1px, transparent 1px);

      background-size: 80px 80px;
      opacity: .15;

      mask-image:
        radial-gradient(circle at center, black 0%, transparent 75%);
    }

    main {
      position: relative;
      z-index: 1;

      width: min(920px, calc(100% - 32px));

      text-align: center;
      padding: 56px 24px;
    }

    .logo-wrap {
      width: min(420px, 86vw);
      margin: 0 auto 34px;

      border-radius: 28px;
      overflow: hidden;

      box-shadow:
        0 0 60px rgba(73,244,255,.25),
        0 0 90px rgba(183,92,255,.20);
    }

    .logo-wrap img {
      width: 100%;
      display: block;
    }

    .eyebrow {
      display: inline-flex;
      align-items: center;
      gap: 10px;

      padding: 10px 16px;

      border: 1px solid rgba(255,255,255,.16);
      border-radius: 999px;

      color: var(--muted);
      background: rgba(255,255,255,.04);

      backdrop-filter: blur(12px);

      margin-bottom: 22px;

      font-size: 14px;
      letter-spacing: .08em;
      text-transform: uppercase;
    }

    .dot {
      width: 8px;
      height: 8px;
      border-radius: 50%;

      background:
        linear-gradient(135deg, var(--cyan), var(--violet));

      box-shadow: 0 0 18px var(--cyan);
    }

    h1 {
      margin: 0;
      font-size: clamp(44px, 8vw, 96px);
      line-height: .92;
      letter-spacing: -0.06em;
    }

    .gradient {
      background:
        linear-gradient(
          90deg,
          var(--cyan),
          #ffffff,
          var(--violet)
        );

      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
    }

    p {
      max-width: 720px;

      margin: 24px auto 0;

      color: var(--muted);

      font-size: clamp(18px, 2.2vw, 24px);
      line-height: 1.5;
    }

    .footer {
      margin-top: 42px;

      font-size: 14px;

      color: rgba(255,255,255,.52);

      letter-spacing: .04em;
    }
  </style>
</head>

<body>
  <main>

    <div class="logo-wrap">
      <img
        src="hyfy-logo.jpeg"
        alt="HYFY Labs"
      />
    </div>

    <div class="eyebrow">
      <span class="dot"></span>
      Coming Soon
    </div>

    <h1>
      <span class="gradient">How You</span><br>
      Find Yours
    </h1>

    <p>
      Products. Communities. Experiences. People.
      HYFY Labs is building tools that help people discover what resonates with them —
      and help organizations understand why.
    </p>

    <div class="footer">
      HYFY Labs
    </div>

  </main>
</body>
</html>
