<!DOCTYPE html>
<html>
<head>
  <title>Certificate Verification</title>
</head>
<body>
  <h2>Smartsolve Institute - Certificate Verification</h2>

  <input type="text" id="certId" placeholder="Enter Certificate ID">
  <button onclick="verify()">Verify</button>

  <p id="result"></p>

  <script>
    const certificates = {
      "SSI001": "Mahesh - Finance Mentorship - 2026",
      "SSI002": "Anita - Excel Course - 2026"
    };

    function verify() {
      const id = document.getElementById("certId").value;
      const result = certificates[id] || "Invalid Certificate ID";
      document.getElementById("result").innerText = result;
    }
  </script>
</body>
</html>
