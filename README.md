<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Top 100 Websites</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f0f4f8;
      color: #333;
      margin: 0;
      padding: 20px;
    }

    header {
      text-align: center;
      padding: 20px;
    }

    h1 {
      margin-bottom: 5px;
    }

    p {
      margin-top: 0;
    }

    #searchInput {
      width: 100%;
      max-width: 400px;
      padding: 10px;
      margin: 20px auto;
      display: block;
      border: 1px solid #ccc;
      border-radius: 6px;
      font-size: 16px;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
      gap: 15px;
    }

    .website-button {
      background-color: #0055aa;
      color: #fff;
      padding: 12px 15px;
      text-align: center;
      text-decoration: none;
      border: none;
      border-radius: 10px;
      font-size: 15px;
      cursor: pointer;
      transition: background-color 0.3s ease;
      display: block;
    }

    .website-button:hover {
      background-color: #ff6600;
    }

    footer {
      text-align: center;
      margin-top: 40px;
      color: #888;
    }
  </style>
</head>
<body>

  <header>
    <h1>🌐 TOP 100 Websites</h1>
    <p>Internet’s Best Resources</p>
  </header>

  <input type="text" id="searchInput" placeholder="Search websites...">

  <div class="grid" id="websiteList">
    <a href="https://www.wolframalpha.com" target="_blank" class="website-button">Wolfram Alpha</a>
    <a href="https://www.typingclub.com" target="_blank" class="website-button">Typing Club</a>
    <a href="https://www.codedex.io" target="_blank" class="website-button">Codedex</a>
    <a href="https://www.ifixit.com" target="_blank" class="website-button">iFixit</a>
    <a href="https://www.math.libretexts.org" target="_blank" class="website-button">Math Libretexts</a>
    <a href="https://www.byjus.com" target="_blank" class="website-button">Byju's</a>
    <a href="https://www.chunkbase.com" target="_blank" class="website-button">Chunkbase</a>
    <a href="https://www.tailornova.com" target="_blank" class="website-button">Tailornova</a>
    <a href="https://www.retrogames.com" target="_blank" class="website-button">RetroGames</a>
    <a href="https://www.pngimg.com" target="_blank" class="website-button">PNG Image</a>
    <a href="https://www.jitter.video" target="_blank" class="website-button">Jitter Video</a>
    <a href="https://www.kiddoworksheets.com" target="_blank" class="website-button">Kiddo Worksheets</a>
    <a href="https://www.fakedetail.com" target="_blank" class="website-button">Fake Details</a>
    <a href="https://www.musclewiki.com" target="_blank" class="website-button">Muscle Wiki</a>
    <a href="https://www.logodiffusion.com" target="_blank" class="website-button">Logo Diffusion</a>
    <a href="https://www.cleanup.pictures" target="_blank" class="website-button">CleanUp Pictures</a>
    <a href="https://www.tv.garden" target="_blank" class="website-button">TV Garden</a>
    <a href="https://www.learn-anything.xyz" target="_blank" class="website-button">Learn Anything</a>
    <a href="https://www.libib.com" target="_blank" class="website-button">Libib</a>
    <a href="https://www.huggingface.co" target="_blank" class="website-button">Hugging Face</a>
    <a href="https://www.gamma.app/create" target="_blank" class="website-button">Gamma App</a>
    <a href="https://www.fakeyou.com" target="_blank" class="website-button">FakeYou</a>
    <a href="https://www.geo-fs.com" target="_blank" class="website-button">Geo-FS</a>
    <a href="https://www.citywalki.com" target="_blank" class="website-button">CityWalki</a>
    <a href="https://www.apob.ai" target="_blank" class="website-button">Apob AI</a>
    <a href="https://www.neal.fun" target="_blank" class="website-button">Neal Fun</a>
    <a href="https://www.yarn.com" target="_blank" class="website-button">Yarn Co</a>
    <a href="https://www.thisoldhouse.com" target="_blank" class="website-button">This Old House</a>
    <a href="https://www.w3schools.com" target="_blank" class="website-button">W3Schools</a>
    <a href="https://www.freecodecamp.org" target="_blank" class="website-button">freeCodeCamp</a>
    <a href="https://www.canva.com" target="_blank" class="website-button">Canva</a>
    <a href="https://www.remove.bg" target="_blank" class="website-button">Remove.bg</a>
    <a href="https://tinyurl.com" target="_blank" class="website-button">TinyURL</a>
    <a href="https://www.pdfescape.com" target="_blank" class="website-button">PDFEscape</a>
    <a href="https://www.youtube.com" target="_blank" class="website-button">YouTube</a>
    <a href="https://www.reddit.com" target="_blank" class="website-button">Reddit</a>
    <a href="https://www.netflix.com" target="_blank" class="website-button">Netflix</a>
    <a href="https://www.notion.so" target="_blank" class="website-button">Notion</a>
    <a href="https://www.trello.com" target="_blank" class="website-button">Trello</a>
    <a href="https://www.todoist.com" target="_blank" class="website-button">Todoist</a>
    <a href="https://www.medium.com" target="_blank" class="website-button">Medium</a>
  </div>

  <footer>
    <p>Created by Nathan Kurgat • Stay Curious, Be Active 🚀</p>
  </footer>

  <script>
    const searchInput = document.getElementById('searchInput');
    const websiteList = document.getElementById('websiteList');
    const links = websiteList.getElementsByTagName('a');

    searchInput.addEventListener('keyup', function () {
      const filter = searchInput.value.toLowerCase();
      for (let i = 0; i < links.length; i++) {
        const txtValue = links[i].textContent || links[i].innerText;
        links[i].style.display = txtValue.toLowerCase().includes(filter) ? "" : "none";
      }
    });
  </script>

</body>
</html>
# websfile
