<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Valentine 💖</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background-color: #ffe6eb;
      margin-top: 100px;
    }

    h1 {
      color: #ff4d6d;
    }

    button {
      padding: 15px 30px;
      font-size: 18px;
      margin: 20px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
    }

    #yesBtn {
      background-color: #ff4d6d;
      color: white;
    }

    #noBtn {
      background-color: #cccccc;
    }
  </style>
</head>
<body>

  <h1>Will you be my Valentine? 💘</h1>

  <button id="yesBtn" onclick="yesClicked()">YES</button>
  <button id="noBtn" onclick="noClicked()">NO</button>

  <script>
    let yesSize = 18;
    let noTexts = [
      "sigee naaaa:<<",
      "loveyyy",
      "babyyyyyyy",
      "Pleaseeee",
      "Love namn ehhh"
    ];
    let noIndex = 0;

    function noClicked() {
      yesSize += 10;
      document.getElementById("yesBtn").style.fontSize = yesSize + "px";

      document.getElementById("noBtn").innerText =
        noTexts[noIndex % noTexts.length];
      noIndex++;
    }

    function yesClicked() {
      document.body.innerHTML =
        "<h1>i Lovee youuuu Bewww</h1>";
    }
  </script>

</body>
</html>
