<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>TikTok Growth Panel</title>

<style>
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #0b1220;
    color: white;
}

.header {
    background: #020617;
    padding: 15px;
    text-align: center;
    font-size: 22px;
    font-weight: bold;
    color: cyan;
}

.container {
    width: 90%;
    max-width: 500px;
    margin: 40px auto;
    background: #111827;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 0 10px cyan;
    text-align: center;
}

input, select, button {
    width: 100%;
    padding: 10px;
    margin-top: 10px;
    border-radius: 5px;
    border: none;
}

button {
    background: cyan;
    font-weight: bold;
    cursor: pointer;
}

button:hover {
    background: #0ea5e9;
}

.status {
    margin-top: 15px;
    font-size: 14px;
    color: #86efac;
}

.features {
    display: flex;
    justify-content: space-between;
    margin-top: 20px;
}

.card {
    background: #020617;
    padding: 10px;
    border-radius: 8px;
    width: 30%;
    text-align: center;
}
</style>

</head>

<body>

<div class="header">TikTok Booster Panel</div>

<div class="container">
    <h2>🚀 TikTok Growth Panel</h2>
    <p>Paste your TikTok video link below:</p>

    <input id="link" type="text" placeholder="Paste TikTok link here">

    <select id="option">
        <option value="views">Increase Views</option>
        <option value="likes">Increase Likes</option>
        <option value="shares">Increase Shares</option>
    </select>

    <button onclick="startProcess()">Start Boost</button>

    <p class="status" id="status"></p>

    <div class="features">
        <div class="card">⚡ Fast</div>
        <div class="card">🔒 Secure</div>
        <div class="card">📊 Live</div>
    </div>
</div>

<script>
function startProcess() {
    let link = document.getElementById("link").value;
    let option = document.getElementById("option").value;
    let status = document.getElementById("status");

    if (link === "") {
        status.innerHTML = "⚠️ Please enter a TikTok link!";
        status.style.color = "red";
        return;
    }

    status.innerHTML = "⏳ Processing " + option + "...";

    setTimeout(() => {
        status.innerHTML = "✅ Done! (Demo version)";
    }, 3000);
}
</script>

</body>
</html>
