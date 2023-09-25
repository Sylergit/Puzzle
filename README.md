# Registration Form
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Animated Registration Form</title>
    <link rel="stylesheet" href="./style.css">
</head>
<body>
        <form action="#">
            <h2>Sign In</h2>
            <div class="inputBox">
                <input type="text" required>
                <label for="#">Username</label>
            </div>
            <div class="inputBox">
                <input type="text" required>
                <label for="#">&nbsp;Password</label>
            </div>
            <div class="check">
                <span>
                    <input type="checkbox">
                    Remember me
                </span>
                <a href="#">Forgot password</a>
            </div>
            <div class="inputBox">
                <input type="submit" value="Sign In">
            </div>
            <p>Don't have an account ? <a href="#">Signup</a></p>
        </form>
        <script>
            let label = document.querySelectorAll('label').forEach(label => {
                label.innerHTML = label.innerText.split('').map((letters, i) => `<span style="transition-delay: ${i * 50}ms" > ${letters}</span>`).join('');
            });
        </script>
</body>
</html>
