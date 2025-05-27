# Hamadapk
Tiktok likes followers and use bilkul free
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>hamadapk.com - Likes & Followers Service</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f6f8;
      margin: 0; padding: 0;
      color: #333;
    }
    header {
      background: #1a73e8;
      color: white;
      padding: 15px 20px;
      text-align: center;
      font-size: 24px;
      font-weight: bold;
    }
    nav {
      background: #1565c0;
      display: flex;
      justify-content: center;
      padding: 10px 0;
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
      font-size: 16px;
    }
    nav a:hover {
      text-decoration: underline;
    }
    .container {
      max-width: 600px;
      background: white;
      margin: 30px auto;
      padding: 20px 30px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      border-radius: 8px;
    }
    h2 {
      text-align: center;
      color: #1565c0;
    }
    form {
      margin-top: 20px;
    }
    label {
      display: block;
      margin-bottom: 8px;
      font-weight: bold;
    }
    input[type="text"], input[type="number"], select {
      width: 100%;
      padding: 10px;
      margin-bottom: 15px;
      border: 1px solid #ccc;
      border-radius: 5px;
      font-size: 15px;
    }
    button {
      background: #1a73e8;
      color: white;
      padding: 12px;
      border: none;
      border-radius: 6px;
      width: 100%;
      font-size: 18px;
      cursor: pointer;
      transition: background 0.3s ease;
    }
    button:hover {
      background: #155db2;
    }
    footer {
      text-align: center;
      padding: 15px 10px;
      margin-top: 40px;
      font-size: 14px;
      color: #777;
    }
  </style>
</head>
<body>
  <header>hamadapk.com</header>
  <nav>
    <a href="#facebook">Facebook Likes</a>
    <a href="#tiktok">TikTok Likes & Followers</a>
  </nav>

  <div class="container" id="facebook">
    <h2>Facebook Likes</h2>
    <form id="fbForm">
      <label for="fbUrl">Facebook Post URL:</label>
      <input type="text" id="fbUrl" placeholder="Enter Facebook post URL" required />

      <label for="fbLikes">Number of Likes:</label>
      <input type="number" id="fbLikes" placeholder="e.g. 1000" min="1" required />

      <button type="submit">Order Facebook Likes</button>
    </form>
  </div>

  <div class="container" id="tiktok">
    <h2>TikTok Likes & Followers</h2>
    <form id="ttForm">
      <label for="ttUsername">TikTok Username:</label>
      <input type="text" id="ttUsername" placeholder="Enter TikTok username" required />

      <label for="ttService">Select Service:</label>
      <select id="ttService" required>
        <option value="">--Choose--</option>
        <option value="likes">Likes</option>
        <option value="followers">Followers</option>
      </select>

      <label for="ttCount">Number of Likes/Followers:</label>
      <input type="number" id="ttCount" placeholder="e.g. 500" min="1" required />

      <button type="submit">Order TikTok Service</button>
    </form>
  </div>

  <footer>
    Contact: +92 300 1234567 | &copy; 2025 hamadapk.com
  </footer>

  <script>
    document.getElementById('fbForm').addEventListener('submit', function(e) {
      e.preventDefault();
      alert('Facebook Likes order received for URL: ' + this.fbUrl.value + ', Likes: ' + this.fbLikes.value);
      this.reset();
    });

    document.getElementById('ttForm').addEventListener('submit', function(e) {
      e.preventDefault();
      alert('TikTok ' + this.ttService.value + ' order received for user: ' + this.ttUsername.value + ', Count: ' + this.ttCount.value);
      this.reset();
    });
  </script>
</body>
</html>
