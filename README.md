<!DOCTYPE html>
<html>
<head>
  <title>Drug Checker</title>
</head>
<body>

<h2>Drug Interaction Checker</h2>

<input type="text" id="drugs" placeholder="Enter drugs (comma separated)">
<button onclick="check()">Check</button>

<p id="result"></p>

<script>
function check() {
  let input = document.getElementById("drugs").value;

  if (input.includes("Ibuprofen") && input.includes("Amoxicillin")) {
    document.getElementById("result").innerText =
      "⚠️ High Risk: Ibuprofen + Amoxicillin → Kidney damage";
  } else {
    document.getElementById("result").innerText =
      "✅ No major risk found";
  }
}
</script>

</body>
</html>
