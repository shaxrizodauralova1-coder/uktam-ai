- `index.html`
- `script.js`
- `style.css`
- `README.md`


<!DOCTYPE html>
<html lang="uz">
<head>
  <meta charset="UTF-8" />
  <title>Utkam AI</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <h1>Utkam AI Chat</h1>
  <div id="chat-box"></div>
  <div id="input-area">
    <input id="user-input" type="text" placeholder="Savolingizni yozing..." />
    <button id="send-btn">Yuborish</button>
  </div>

  <script src="script.js"></script>
</body>
</html>


body {
  font-family: Arial, sans-serif;
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
}
#chat-box {
  border: 1px solid #ccc;
  padding: 10px;
  height: 400px;
  overflow-y: auto;
  margin-bottom: 10px;
}
.message {
  margin: 5px 0;
}
.message.user {
  text-align: right;
  color: blue;
}
.message.ai {
  text-align: left;
  color: green;
}
#input-area {
  display: flex;
  gap: 10px;
}
#user-input {
  flex: 1;
  padding: 8px;
}
