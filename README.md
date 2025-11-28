# -2400032702--SkillEndSemExam
College Portal Theme Switcher Using Context API


<!DOCTYPE html>
<html>
<head>
    <title>KL Student Portal - Theme Switcher</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            transition: 0.3s;
            text-align: center;
            padding: 40px;
        }

        .light-theme {
            background-color: white;
            color: black;
        }

        .dark-theme {
            background-color: #222;
            color: white;
        }

        button {
            padding: 10px 18px;
            border: none;
            cursor: pointer;
            font-size: 16px;
            margin-top: 20px;
            border-radius: 5px;
        }

        button:hover {
            opacity: 0.8;
        }
    </style>
</head>

<body class="light-theme">

    <h2>KL University Student Portal</h2>
    <p id="status">Current Theme: Light</p>

    <button id="toggleBtn">Toggle Theme</button>

    <script>
        const body = document.body;
        const status = document.getElementById("status");
        const toggleBtn = document.getElementById("toggleBtn");

        toggleBtn.addEventListener("click", () => {
            if (body.classList.contains("light-theme")) {
                body.classList.replace("light-theme", "dark-theme");
                status.textContent = "Current Theme: Dark";
            } else {
                body.classList.replace("dark-theme", "light-theme");
                status.textContent = "Current Theme: Light";
            }
        });
    </script>

</body>
</html>
