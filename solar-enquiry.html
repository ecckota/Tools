<?php
// PHP CODE TO HANDLE FORM SUBMISSION
if ($_SERVER['REQUEST_METHOD'] === 'POST') {
    // Sanitize inputs
    $name = htmlspecialchars($_POST['name']);
    $email = htmlspecialchars($_POST['email']);
    $phone = htmlspecialchars($_POST['phone']);
    $service = htmlspecialchars($_POST['service']);
    $square_footage = htmlspecialchars($_POST['square_footage']);

    // Validate inputs
    if (empty($name) || empty($email) || empty($phone) || empty($service)) {
        $error = "All fields are required!";
    } else {
        // Connect to MySQL database (Update credentials!)
        $servername = "localhost";
        $username = "root";
        $password = "";
        $dbname = "solar_leads";

        $conn = new mysqli($servername, $username, $password, $dbname);
        if ($conn->connect_error) {
            die("Connection failed: " . $conn->connect_error);
        }

        // Insert lead into database
        $stmt = $conn->prepare("INSERT INTO leads (name, email, phone, service, square_footage) VALUES (?, ?, ?, ?, ?)");
        $stmt->bind_param("ssssi", $name, $email, $phone, $service, $square_footage);
        $stmt->execute();
        $stmt->close();
        $conn->close();

        // Redirect to thank-you page
        header("Location: thank_you.html");
        exit();
    }
}
?>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Solar Lead Generation</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f8ff;
        }
        .header {
            background-color: #1e90ff;
            color: white;
            padding: 20px;
            text-align: center;
        }
        .container {
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
        }
        .lead-form {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        .form-group {
            margin-bottom: 15px;
        }
        input, select {
            width: 100%;
            padding: 10px;
            margin: 5px 0;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        button {
            background: #1e90ff;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background: #0066cc;
        }
        .error {
            color: red;
            margin-bottom: 10px;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>Switch to Solar Energy</h1>
        <p>Get a Free Quote Today!</p>
    </div>

    <div class="container">
        <div class="lead-form">
            <h2>Request a Solar Consultation</h2>
            <?php if (isset($error)) echo "<p class='error'>$error</p>"; ?>
            <form method="POST">
                <div class="form-group">
                    <input type="text" name="name" placeholder="Full Name" required>
                </div>
                <div class="form-group">
                    <input type="email" name="email" placeholder="Email Address" required>
                </div>
                <div class="form-group">
                    <input type="tel" name="phone" placeholder="Phone Number" required>
                </div>
                <div class="form-group">
                    <select name="service" required>
                        <option value="">Select Service</option>
                        <option value="residential">Residential Solar Installation</option>
                        <option value="commercial">Commercial Solar Solutions</option>
                    </select>
                </div>
                <div class="form-group">
                    <input type="number" name="square_footage" placeholder="Approximate Square Footage" required>
                </div>
                <button type="submit">Get Free Quote</button>
            </form>
        </div>
    </div>

    <script>
        // Basic phone number validation
        document.querySelector('form').addEventListener('submit', function(e) {
            const phone = document.querySelector('input[name="phone"]').value;
            if (phone.length < 10) {
                alert('Please enter a valid phone number.');
                e.preventDefault();
            }
        });
    </script>
</body>
</html>
