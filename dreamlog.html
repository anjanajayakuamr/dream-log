# dream-log
<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Dream Log 🌙</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom, #1e1b4b, #6d28d9);
      color: white;
      padding: 2rem;
    }
    h1 {
      text-align: center;
      font-size: 2.5rem;
      margin-bottom: 1.5rem;
    }
    form {
      background-color: rgba(255, 255, 255, 0.1);
      padding: 1rem;
      border-radius: 10px;
      max-width: 600px;
      margin: 0 auto 2rem auto;
    }
    input, textarea {
      width: 100%;
      padding: 0.75rem;
      margin-bottom: 1rem;
      border: none;
      border-radius: 5px;
      background-color: rgba(255, 255, 255, 0.2);
      color: white;
    }
    input::placeholder, textarea::placeholder {
      color: rgba(255, 255, 255, 0.6);
    }
    button {
      background-color: #4f46e5;
      padding: 0.75rem 1.5rem;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    .dream-card {
      background-color: rgba(255, 255, 255, 0.1);
      padding: 1rem;
      border-radius: 10px;
      margin-bottom: 1rem;
      max-width: 600px;
      margin-left: auto;
      margin-right: auto;
    }
    .dream-card h2 {
      margin: 0 0 0.5rem 0;
    }
    .dream-card p {
      margin-bottom: 0.5rem;
    }
    .tags {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
    }
    .tag {
      background-color: #a855f7;
      padding: 0.25rem 0.75rem;
      border-radius: 20px;
      font-size: 0.9rem;
    }
    .date {
      font-size: 0.8rem;
      opacity: 0.7;
      text-align: right;
    }
    #exportButton {
      display: block;
      margin: 0 auto 2rem auto;
      background-color: #10b981;
    }
  </style>
</head>
<body>  <h1>🌙 Dream Log</h1>  <form id="dreamForm">
    <input type="text" id="dreamTitle" placeholder="Dream Title" required />
    <textarea id="dreamDescription" placeholder="Describe your dream..." rows="4" required></textarea>
    <input type="text" id="dreamTags" placeholder="Tags (e.g., flying, water, lucid)" />
    <button type="submit">Add Dream</button>
  </form><button id="exportButton" onclick="exportDreams()">Export Dreams</button>

  <div id="dreamsContainer"></div>  <script>
    const form = document.getElementById('dreamForm');
    const dreamsContainer = document.getElementById('dreamsContainer');

    function formatDate(date) {
      return new Date(date).toLocaleDateString();
    }

    function createDreamCard(dream) {
      const card = document.createElement('div');
      card.className = 'dream-card';

      card.innerHTML = 
        <h2>${dream.title}</h2>
        <p>${dream.description}</p>
        <div class="tags">
          ${dream.tags.map(tag => <span class="tag">#${tag}</span>).join('')}
        </div>
        <div class="date">${formatDate(dream.date)}</div>
      ;

      dreamsContainer.prepend(card);
    }

    form.addEventListener('submit', (e) => {
      e.preventDefault();

      const title = document.getElementById('dreamTitle').value.trim();
      const description = document.getElementById('dreamDescription').value.trim();
      const tags = document.getElementById('dreamTags').value.trim().split(',').map(t => t.trim()).filter(Boolean);

      if (!title || !description) {
        alert("Please enter both a title and a description for your dream.");
        return;
      }

      const newDream = {
        title,
        description,
        tags,
        date: new Date()
      };

      createDreamCard(newDream);
      saveDream(newDream);
      form.reset();
    });

    function saveDream(dream) {
      const saved = JSON.parse(localStorage.getItem('dreams') || '[]');
      saved.push(dream);
      localStorage.setItem('dreams', JSON.stringify(saved));
    }

    function loadDreams() {
      const saved = JSON.parse(localStorage.getItem('dreams') || '[]');
      saved.reverse().forEach(createDreamCard);
    }

    function exportDreams() {
      const dreams = localStorage.getItem('dreams');
      if (!dreams || dreams.length === 0) {
        alert("No dreams to export.");
        return;
      }
      const blob = new Blob([dreams], { type: 'application/json' });
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url;
      a.download = 'dreams.json';
      a.click();
    }

    loadDreams();
  </script></body>
</html>
