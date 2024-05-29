# Solution By Zulu

1. Set up the solution to run the API and WebApp simultaneously.
2. Put a break point in ForecastService.cs to identify the problem.
3. I identified that the problem was that the URL parameter is null because it is not in the settings.
4. Add the Url parameter in the correct section in appsettings.json:

"ApiSettings": {
  "Url": "http://localhost:5104/"
}

5. Run the App and test

It works!

------------------------------------------------------------------------------------------------------------------------------------------------------

# TestApp

Display the data when clicking on this link

![image](https://github.com/macaldinho/TestApp/assets/5600418/72004bd2-690c-44de-a5bc-ed69ee2c456e)

Update the code to use the commented code

![image](https://github.com/macaldinho/TestApp/assets/5600418/2391829e-84a1-44f3-8c96-6df9110ef9cd)

Extra points

    Containerize the apps with docker
