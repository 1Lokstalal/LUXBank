<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>LUXBANK - Console</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #0f0f0f;
      color: white;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    h1 {
      background: linear-gradient(to right, gold, orange);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      margin-top: 30px;
    }
    .login, .console {
      background-color: #1e1e1e;
      padding: 20px;
      border-radius: 15px;
      box-shadow: 0 0 15px rgba(255, 215, 0, 0.4);
      width: 90%;
      max-width: 500px;
      margin-top: 20px;
    }
    input {
      width: 100%;
      padding: 10px;
      margin: 8px 0;
      border: none;
      border-radius: 8px;
      background: #2c2c2c;
      color: white;
    }
    button {
      width: 100%;
      padding: 10px;
      background-color: gold;
      border: none;
      color: black;
      font-weight: bold;
      border-radius: 8px;
      cursor: pointer;
    }
    #output {
      white-space: pre-wrap;
      margin-top: 15px;
      background-color: #111;
      padding: 10px;
      border-radius: 8px;
      max-height: 200px;
      overflow-y: auto;
    }
  </style>
</head>
<body>

  <h1>🏦 LUXBANK - Your Digital Power 🪙</h1>

  <div class="login" id="loginBox">
    <h2>تسجيل الدخول</h2>
    <input type="text" id="username" placeholder="Username">
    <input type="password" id="password" placeholder="Password">
    <input type="text" id="code" placeholder="Security Code">
    <button onclick="login()">Login</button>
  </div>

  <div class="console" id="consoleBox" style="display: none;">
    <h2>Welcome to LUXBANK Console</h2>
    <p>رتبتك: <span id="userRank"></span></p>
    <input type="text" id="commandInput" placeholder="Enter Command">
    <button onclick="runCommand()">Send Command</button>
    <div id="output"></div>
  </div>

  <script>
    const users = {
      "talal": { password: "113344", code: "113344", rank: "OWNER", money: 0 },
      "john": { password: "1234", code: "000", rank: "MANAGER", money: 100 }
    };

    const ranks = ["OWNER", "CEO", "MANAGER", "ADMIN", "MEMBER"];

    let currentUser = null;

    function login() {
      const user = document.getElementById("username").value;
      const pass = document.getElementById("password").value;
      const code = document.getElementById("code").value;

      if (users[user] && users[user].password === pass && users[user].code === code) {
        currentUser = user;
        document.getElementById("loginBox").style.display = "none";
        document.getElementById("consoleBox").style.display = "block";
        document.getElementById("userRank").innerText = users[user].rank;
        printOutput(`✅ تم تسجيل الدخول كـ ${user}`);
      } else {
        alert("بيانات الدخول غير صحيحة");
      }
    }

    function runCommand() {
      const input = document.getElementById("commandInput").value.trim();
      const args = input.split(" ");
      const cmd = args[0];

      const userRank = users[currentUser].rank;
      const allowedRanks = ["CEO", "MANAGER", "OWNER"];

      function hasPermission() {
        return allowedRanks.includes(userRank);
      }

      switch (cmd) {
        case "$addmoney":
          if (!hasPermission()) return noPerm();
          if (!users[args[1]]) return userNotFound();
          users[args[1]].money += parseInt(args[2]);
          printOutput(`💰 Successfully Added To ${args[2]} Account ${args[1]}`);
          break;

        case "$removemoney":
          if (!hasPermission()) return noPerm();
          if (!users[args[1]]) return userNotFound();
          users[args[1]].money -= parseInt(args[2]);
          printOutput(`💸 Successfully Took ${args[2]} From ${args[1]}`);
          break;

        case "$giverank":
          if (!hasPermission()) return noPerm();
          if (!users[args[1]]) return userNotFound();
          users[args[1]].rank = args[2];
          printOutput(`🎖️ Successfully Gave The Rank ${args[2]} ${args[1]}`);
          break;

        case "$takerank":
          if (!hasPermission()) return noPerm();
          if (!users[args[1]]) return userNotFound();
          users[args[1]].rank = "MEMBER";
          printOutput(`🧾 You Have Been Successfully Took The Rank ${args[1]} MEMBER`);
          break;

        case "$createrank":
          if (!hasPermission()) return noPerm();
          if (ranks.includes(args[1])) {
            printOutput("⚠️ That Rank Is Already Created");
          } else {
            ranks.push(args[1]);
            printOutput(`✅ You Have Been Successfully Created The Rank ${args[1]}`);
          }
          break;

        case "$deleterank":
          if (!hasPermission()) return noPerm();
          const index = ranks.indexOf(args[1]);
          if (index > -1) {
            ranks.splice(index, 1);
            printOutput(`🗑️ You Have Been Successfully Deleted The Rank ${args[1]}`);
          } else {
            printOutput("❌ That Rank Not Found");
          }
          break;
        case "$pay":
    if (!users[args[1]]) return userNotFound();
    const amount = parseInt(args[2]);
    if (isNaN(amount) || amount <= 0) return printOutput("❌ Enter The Transfer Amount");
    if (users[currentUser].money < amount) return printOutput("❌ You Dont Have Enough Money");

  users[currentUser].money -= amount;
  users[args[1]].money += amount;
  printOutput(`✅ ${amount} Has Been Successfully Paid! ${args[1]}`);
  break;
      
  case "$showbalance":
    printOutput(`Your Account Balance: ${users[currentUser].money}`);
    break;



        case "$developer":
          printOutput("👨‍💻 This Bank System Was Developed By: Talal (1Loks)");
          break;

      case "$discord":
          printOutput("🎟️ Discord Server Link : https://discord.gg/QVbVYhUu 🛡️");
          break;

      // حفظ البيانات
function saveData() {
  localStorage.setItem("lux_users", JSON.stringify(users));
  localStorage.setItem("lux_ranks", JSON.stringify(ranks));
  localStorage.setItem("lux_currentUser", currentUser);
}

// تحميل البيانات
function loadData() {
  const savedUsers = localStorage.getItem("lux_users");
  const savedRanks = localStorage.getItem("lux_ranks");
  const savedCurrentUser = localStorage.getItem("lux_currentUser");

  if (savedUsers) users = JSON.parse(savedUsers);
  if (savedRanks) ranks = JSON.parse(savedRanks);
  if (savedCurrentUser) currentUser = savedCurrentUser;
}

        default:
          printOutput("❌ Command Not Found");
      }
    }

    function printOutput(text) {
      document.getElementById("output").innerText += text + "\n";
    }

    function noPerm() {
      printOutput("🚫 You Dont Have Access To Use This Command ");
    }

    function userNotFound() {
      printOutput("❌ User Not Found!");
    }
  </script>
</body>
</html>

