<!DOCTYPE html>
<html>
  <head>
    <title>Greetings and Advice</title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  </head>
  <body>
    <h1 id="greeting"></h1>
    <p id="advice"></p>

    <script>
      // Get the current date and time
      const now = new Date();

      // Get the hour of the day (0-23)
      const hour = now.getHours();

      // Get the greeting based on the hour of the day
      let greeting;
      if (hour < 12) {
        greeting = "Good morning";
      } else if (hour < 18) {
        greeting = "Good afternoon";
      } else {
        greeting = "Good evening";
      }

      // Get the username from the user
      const username = prompt("What's your name?");

      // Set the greeting text
      const greetingElement = document.getElementById("greeting");
      greetingElement.innerText = `${greeting}, ${username}, you look great today!`;

      // Give the user some advice
      const adviceElement = document.getElementById("advice");
      const advice = "Remember to stay hydrated and take breaks throughout the day.";
      adviceElement.innerText = advice;
    </script>
  </body>
</html>
