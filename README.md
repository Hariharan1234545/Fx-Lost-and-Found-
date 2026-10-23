```
/* FRANCIS XAVIER ENGINEERING COLLEGE THEME */
:root {
  --bg: #061b36;
  --panel: #0b2c52;
  --panel2: #103b69;
  --line: rgba(255, 255, 255, 0.14);
  --text: #f5f8ff;
  --muted: #bdcde2;
  --cyan: #65b5ff;
  --blue: #0755a5;
  --green: #91b45b;
  --orange: #ffb600;
  --danger: #ff7d89;
  --shadow: 0 18px 55px rgba(0, 0, 0, 0.28);
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  color: var(--text);
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.6;
  background:
    linear-gradient(rgba(4, 24, 48, 0.94), rgba(4, 24, 48, 0.97)),
    url("fxec-logo.png") center 180px / min(75vw, 650px) auto
      no-repeat fixed,
    #061b36;
}

/* Official college logo watermark */
body::before {
  content: "";
  position: fixed;
  inset: 0;
  background: url("fxec-logo.png") center center / min(70vw, 600px) auto
    no-repeat;
  opacity: 0.055;
  pointer-events: none;
  z-index: -1;
}

/* College-branded header */
header {
  background: rgba(5, 35, 70, 0.96);
  border-bottom: 3px solid var(--orange);
  backdrop-filter: blur(18px);
}

/* College banner */
.college-banner {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 12px 18px;
  background: #ffffff;
  border-bottom: 4px solid var(--orange);
}

.college-banner img {
  display: block;
  width: min(820px, 100%);
  max-height: 145px;
  object-fit: contain;
}

/* Cards and panels */
.card,
.panel,
.stat-card,
.report-card {
  background: rgba(11, 44, 82, 0.94);
  border: 1px solid var(--line);
  border-radius: 18px;
  box-shadow: var(--shadow);
}

/* Buttons */
button,
.btn,
.primary-button {
  background: linear-gradient(135deg, #0755a5, #0878c9);
  color: #ffffff;
  border: 1px solid rgba(255, 255, 255, 0.16);
  border-radius: 10px;
  transition: 0.2s ease;
}

button:hover,
.btn:hover,
.primary-button:hover {
  background: linear-gradient(135deg, #ffb600, #e99500);
  color: #061b36;
  transform: translateY(-2px);
}

/* Headings and highlights */
h1,
h2,
h3 {
  color: #ffffff;
}

.highlight,
.accent,
.logo-accent {
  color: var(--orange);
}

a {
  color: #82c7ff;
}

input,
select,
textarea {
  background: #071f3c;
  color: #ffffff;
  border: 1px solid rgba(255, 255, 255, 0.2);
  border-radius: 10px;
}

input:focus,
select:focus,
textarea:focus {
  outline: 2px solid var(--orange);
  border-color: var(--orange);
}

/* Gold separators */
hr,
.section-divider {
  border: 0;
  border-top: 2px solid rgba(255, 182, 0, 0.55);
}

/* Keep the watermark subtle on mobile */
@media (max-width: 600px) {
  body {
    background-attachment: scroll;
  }

  body::before {
    background-size: 90vw auto;
    opacity: 0.035;
  }

  .college-banner img {
    max-height: 100px;
  }
}
```
