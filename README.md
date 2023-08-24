# hello-world
My first repository on GitHub
<!DOCTYPE html>
<html>
  <head>
    <base target="_top">
  </head>
  <body>
    <h1>Google Apps Script Example</h1>
    <button id="getData">Get Data</button>
    <p id="output"></p>
    
    <script>
      // Function to call Google Apps Script function
      function getDataFromGoogleAppsScript() {
        google.script.run.withSuccessHandler(displayData).getData();
      }

      // Function to display data received from Google Apps Script
      function displayData(data) {
        document.getElementById('output').textContent = data;
      }

      // Add a click event listener to the button
      document.getElementById('getData').addEventListener('click', getDataFromGoogleAppsScript);
    </script>
  </body>
</html>
