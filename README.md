[supporter_moderator_bewerbung.html](https://github.com/user-attachments/files/34754592/supporter_moderator_bewerbung.html)<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="theme-color" content="#101827">
  <title>Supporter / Moderator Bewerbung</title>
  <style>
    :root {
      --bg: #0b1120;
      --panel: #121c2e;
      --panel-2: #17243a;
      --text: #eef4ff;
      --muted: #a7b4c9;
      --line: #2b3b55;
      --accent: #60a5fa;
      --accent-2: #3b82f6;
      --good: #86efac;
    }
    * { box-sizing: border-box; }
    body {
      margin: 0; color: var(--text);
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, Segoe UI, sans-serif;
      background:
        radial-gradient(ellipse at 15% 0%, rgba(59,130,246,.18), transparent 36rem),
        radial-gradient(ellipse at 100% 20%, rgba(14,165,233,.10), transparent 32rem),
        var(--bg);
      line-height: 1.6;
    }
    .wrap { width: min(900px, calc(100% - 32px)); margin: 0 auto; padding: 52px 0 72px; }
    header { text-align: center; margin-bottom: 34px; }
    .eyebrow {
      display: inline-block; padding: 6px 12px; border: 1px solid #34527a;
      border-radius: 999px; color: #bfdbfe; background: rgba(59,130,246,.10);
      font-size: .78rem; font-weight: 700; letter-spacing: .12em; text-transform: uppercase;
    }
    h1 { margin: 16px 0 8px; font-size: clamp(2rem, 5vw, 3.1rem); line-height: 1.12; }
    header p { margin: 0 auto; max-width: 650px; color: var(--muted); }
    form { display: grid; gap: 20px; }
    fieldset, .section {
      min-width: 0; margin: 0; padding: 25px;
      border: 1px solid var(--line); border-radius: 18px;
      background: linear-gradient(145deg, rgba(23,36,58,.96), rgba(18,28,46,.96));
      box-shadow: 0 14px 35px rgba(0,0,0,.16);
    }
    legend, h2 { padding: 0; margin: 0 0 18px; font-size: 1.2rem; font-weight: 750; }
    legend { float: left; width: 100%; }
    legend + * { clear: both; }
    .number { color: var(--accent); margin-right: 8px; }
    .grid { display: grid; grid-template-columns: repeat(2, minmax(0,1fr)); gap: 16px; clear: both; }
    .field { display: flex; flex-direction: column; gap: 7px; min-width: 0; }
    .full { grid-column: 1 / -1; }
    label, .question { font-weight: 650; font-size: .94rem; }
    .hint { color: var(--muted); font-size: .84rem; margin-top: -3px; }
    input[type="text"], input[type="number"], textarea, select {
      width: 100%; color: var(--text); background: #0d1728;
      border: 1px solid #354761; border-radius: 10px; padding: 12px 13px;
      font: inherit; outline: none; transition: border-color .2s, box-shadow .2s;
    }
    textarea { min-height: 100px; resize: vertical; }
    input:focus, textarea:focus, select:focus {
      border-color: var(--accent); box-shadow: 0 0 0 3px rgba(96,165,250,.15);
    }
    .choice { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 8px; }
    .choice label {
      display: inline-flex; align-items: center; gap: 8px; cursor: pointer;
      padding: 8px 15px; border: 1px solid #3a4d69; border-radius: 10px;
      background: #0d1728; font-weight: 600;
    }
    input[type="radio"] { accent-color: var(--accent-2); width: 17px; height: 17px; }
    .questions { display: grid; gap: 19px; clear: both; }
    .q { padding-bottom: 17px; border-bottom: 1px solid rgba(72,94,124,.45); }
    .q:last-child { border-bottom: 0; padding-bottom: 0; }
    .q .field { margin-top: 10px; }
    .required-note { color: var(--muted); font-size: .86rem; margin: 0; }
    .actions { display: flex; flex-direction: column; align-items: center; gap: 12px; }
    button {
      border: 0; border-radius: 12px; padding: 14px 28px; min-width: 230px;
      background: linear-gradient(135deg, #60a5fa, #2563eb); color: white;
      font: inherit; font-weight: 800; cursor: pointer;
      box-shadow: 0 10px 25px rgba(37,99,235,.25); transition: transform .2s, filter .2s;
    }
    button:hover { transform: translateY(-2px); filter: brightness(1.08); }
    button:focus-visible { outline: 3px solid #bfdbfe; outline-offset: 3px; }
    #status { color: var(--good); text-align: center; min-height: 1.5em; }
    footer { color: var(--muted); text-align: center; font-size: .82rem; margin-top: 28px; }
    @media (max-width: 640px) {
      .wrap { width: min(100% - 22px, 900px); padding-top: 32px; }
      fieldset, .section { padding: 19px 16px; }
      .grid { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>
  <main class="wrap">
    <header>
      <span class="eyebrow">Team-Bewerbung</span>
      <h1>Supporter / Moderator Bewerbung</h1>
      <p>Du möchtest unser Team unterstützen? Fülle das Formular bitte ehrlich und vollständig aus. Wir freuen uns darauf, dich kennenzulernen.</p>
    </header>

    <form id="application">
      <fieldset>
        <legend><span class="number">01</span>Allgemeines</legend>
        <div class="grid">
          <div class="field">
            <label for="alias">Name / Alias *</label>
            <input id="alias" name="Name / Alias" type="text" required>
          </div>
          <div class="field">
            <label for="age">Alter *</label>
            <input id="age" name="Alter" type="number" min="13" max="99" required>
          </div>
          <div class="field">
            <label for="discord">Discord-Tag *</label>
            <input id="discord" name="Discord-Tag" type="text" placeholder="z. B. name" required>
          </div>
          <div class="field">
            <label for="player">Spielername auf dem Server *</label>
            <input id="player" name="Spielername auf dem Server" type="text" required>
          </div>
          <div class="field full">
            <label for="time">Wie lange spielst du schon bei uns und wie viele Spielstunden hast du? *</label>
            <textarea id="time" name="Spielzeit" required placeholder="Beschreibe deine bisherige Spielzeit ..."></textarea>
          </div>
          <div class="field full">
            <span class="question">Hast du aktuell Sanktionen, Verwarnungen oder Bans (bei uns oder anderswo)? *</span>
            <div class="choice">
              <label><input type="radio" name="Aktuelle Sanktionen" value="Ja" required> Ja</label>
              <label><input type="radio" name="Aktuelle Sanktionen" value="Nein"> Nein</label>
            </div>
            <label for="sanctions">Falls ja, bitte kurz erläutern.</label>
            <textarea id="sanctions" name="Details zu Sanktionen" placeholder="Was ist passiert und wann?"></textarea>
          </div>
          <div class="field full">
            <span class="question">Bist du aktuell in anderen Serverteams aktiv? *</span>
            <div class="choice">
              <label><input type="radio" name="In anderen Serverteams aktiv" value="Ja" required> Ja</label>
              <label><input type="radio" name="In anderen Serverteams aktiv" value="Nein"> Nein</label>
            </div>
            <label for="otherteams">Falls ja, auf welchen Servern und in welcher Rolle?</label>
            <textarea id="otherteams" name="Andere Serverteams" placeholder="Deine Angaben ..."></textarea>
          </div>
        </div>
      </fieldset>

      <fieldset>
        <legend><span class="number">02</span>Erfahrung</legend>
        <div class="questions">
          <div class="q">
            <span class="question">Hast du Erfahrung im Supportbereich oder als Moderator, auch auf anderen Servern? *</span>
            <div class="choice">
              <label><input type="radio" name="Support-Erfahrung" value="Ja" required> Ja</label>
              <label><input type="radio" name="Support-Erfahrung" value="Nein"> Nein</label>
            </div>
            <div class="field">
              <label for="experience">Wie lange und in welcher Rolle? Warum hast du dort aufgehört?</label>
              <textarea id="experience" name="Details zur Support-Erfahrung" required></textarea>
            </div>
          </div>
          <div class="q">
            <div class="field">
              <label for="rp">Hast du RP-Erfahrung in verschiedenen Rollen (Zivilist, Fraktion, Gang, Staatsdienst)? *</label>
              <textarea id="rp" name="RP-Erfahrung" required placeholder="Nenne deine bisherigen Rollen und Erfahrungen ..."></textarea>
            </div>
          </div>
        </div>
      </fieldset>

      <fieldset>
        <legend><span class="number">03</span>Motivation</legend>
        <div class="questions">
          <div class="q"><div class="field">
            <label for="motivation">Warum möchtest du Supporter / Moderator werden? *</label>
            <textarea id="motivation" name="Motivation" required></textarea>
          </div></div>
          <div class="q"><div class="field">
            <label for="offer">Was kannst du dem Team bieten, was aktuell vielleicht noch fehlt? *</label>
            <textarea id="offer" name="Was du dem Team bietest" required></textarea>
          </div></div>
          <div class="q"><div class="field">
            <label for="future">Wo siehst du dich in 3 Monaten im Team? *</label>
            <textarea id="future" name="Ziele in 3 Monaten" required></textarea>
          </div></div>
          <div class="q"><div class="field">
            <label for="goodstaff">Was macht für dich einen guten Supporter aus? *</label>
            <textarea id="goodstaff" name="Guter Supporter" required></textarea>
          </div></div>
        </div>
      </fieldset>

      <fieldset>
        <legend><span class="number">04</span>Szenarien</legend>
        <p class="required-note">Beschreibe jeweils, wie du in der Situation handeln würdest.</p>
        <div class="questions" style="margin-top:18px">
          <div class="q"><div class="field">
            <label for="scenario1">Ein Spieler beschuldigt einen anderen des Powergamings, es gibt keine Beweise. Wie gehst du vor? *</label>
            <textarea id="scenario1" name="Szenario: Powergaming" required></textarea>
          </div></div>
          <div class="q"><div class="field">
            <label for="scenario2">Ein langjähriger Freund von dir bricht eine Regel. Was machst du? *</label>
            <textarea id="scenario2" name="Szenario: Freund bricht Regel" required></textarea>
          </div></div>
          <div class="q"><div class="field">
            <label for="scenario3">Ein Spieler beleidigt dich im Ticket oder Support-Talk. Wie reagierst du? *</label>
            <textarea id="scenario3" name="Szenario: Beleidigung" required></textarea>
          </div></div>
          <div class="q"><div class="field">
            <label for="scenario4">Du bekommst gleichzeitig 3 Tickets. Wie priorisierst du? *</label>
            <textarea id="scenario4" name="Szenario: Drei Tickets" required></textarea>
          </div></div>
          <div class="q"><div class="field">
            <label for="scenario5">Ein Teammitglied missbraucht seine Rechte. Was tust du? *</label>
            <textarea id="scenario5" name="Szenario: Rechte-Missbrauch" required></textarea>
          </div></div>
          <div class="q"><div class="field">
            <label for="scenario6">Ein Spieler fordert eine Entschädigung für verlorene Items. Wie prüfst du das? *</label>
            <textarea id="scenario6" name="Szenario: Item-Entschädigung" required></textarea>
          </div></div>
          <div class="q"><div class="field">
            <label for="scenario7">Ein Spieler droht mit Verlassen des Servers, wenn du ihn nicht entbannst. Wie reagierst du? *</label>
            <textarea id="scenario7" name="Szenario: Entbannungs-Drohung" required></textarea>
          </div></div>
          <div class="q"><div class="field">
            <label for="scenario8">Du bist dir bei einer Entscheidung unsicher. Was machst du? *</label>
            <textarea id="scenario8" name="Szenario: Unsichere Entscheidung" required></textarea>
          </div></div>
        </div>
      </fieldset>

      <p class="required-note">* Pflichtfelder. Mit dem Absenden wird deine Bewerbung als Textdatei auf deinem Gerät gespeichert.</p>
      <div class="actions">
        <button type="submit">Bewerbung absenden</button>
        <div id="status" role="status" aria-live="polite"></div>
      </div>
    </form>
    <footer>Bitte gib nur richtige und vollständige Angaben an.</footer>
  </main>

  <script>
    const form = document.getElementById('application');
    const status = document.getElementById('status');

    form.addEventListener('submit', (event) => {
      event.preventDefault();
      if (!form.reportValidity()) return;

      const data = new FormData(form);
      const lines = ['SUPPORTER / MODERATOR BEWERBUNG', '================================', ''];
      const seen = new Set();

      for (const [key, value] of data.entries()) {
        if (seen.has(key)) continue;
        seen.add(key);
        const values = data.getAll(key).join(', ');
        lines.push(key.toUpperCase(), values || 'Keine Angabe', '');
      }

      const blob = new Blob([lines.join('\n')], { type: 'text/plain;charset=utf-8' });
      const url = URL.createObjectURL(blob);
      const link = document.createElement('a');
      link.href = url;
      link.download = 'Supporter-Moderator-Bewerbung.txt';
      document.body.appendChild(link);
      link.click();
      link.remove();
      URL.revokeObjectURL(url);

      status.textContent = 'Vielen Dank! Deine Bewerbung wurde als Textdatei gespeichert.';
      form.reset();
    });
  </script>
</body>
</html>
