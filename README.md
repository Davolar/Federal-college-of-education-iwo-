<!DOCTYPE html>
<html>
<head>
    <title>E-Voting Portal</title>
</head>
<body>
    <h2>Welcome to E-Voting Portal</h2>

    <input type="text" id="voterId" placeholder="Enter Voter ID">
    <button onclick="login()">Login</button>

    <script>
        function login() {
            const voterId = document.getElementById("voterId").value;
            if(voterId === "") {
                alert("Enter Voter ID");
                return;
            }
            localStorage.setItem("voterId", voterId);
            window.location.href = "vote.html";
        }
    </script>
</body>
</html>
