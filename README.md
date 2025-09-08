<!DOCTYPE html>
<html>
<head>
  <title>解锁小程序</title>
  <style>
    .hidden { display: none; }
  </style>
</head>
<body>
  <input type="text" id="password" placeholder="输入密码">
  <button onclick="checkPassword()">解锁</button>
  <div id="secretContent" class="hidden">
    <h2>解锁成功！</h2>
    <p>这里是隐藏内容...</p>
  </div>
 
  <script>
    function checkPassword() {
      const password = document.getElementById("password").value;
      const secretContent = document.getElementById("secretContent");
      // 预设密码（可改为后端API调用）
      if (password === "m4A1") {
        secretContent.classList.remove("hidden");
      } else {
        alert("密码错误！");
      }
    }
  </script>
</body>
</html>
