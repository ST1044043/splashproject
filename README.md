
Samkelo Radebe ST10440433
Purpose of creating weather
The purpose of the weather app is to provide users with accurate and convenient access to weather forecasts for the upcoming week. By utilizing arrays to manage the weekly weather data, the app aims to organize and present this information in an easy-to-understand format. Users can quickly glance at the app to check the forecast for each day of the week, allowing them to plan their activities accordingly. The app may also include additional features such as current weather conditions, hourly forecasts, and customizable alerts to enhance user experience and utility.

Pseudocode
 Start
// Weather App Splash Screen Pseudocode

// Define constants for UI elements
CONSTANT LOGO_IMAGE = "logo.png"
CONSTANT BUTTON_IMAGE = "button.png"

// Define variables for weather data
VARIABLE weeklyWeatherArray[7]
VARIABLE averageTemperature

// Load logo and button images
FUNCTION loadImages():
    // Load logo image
    logo = loadImage(LOGO_IMAGE)
    // Load button image
    button = loadImage(BUTTON_IMAGE)

// Display splash screen UI
FUNCTION displaySplashScreen():
    // Display logo
    displayImage(logo, x=100, y=100)
    // Display app title
    displayText("Weather App", x=150, y=50)
    // Display weekly weather summary
    FOR i FROM 0 TO 6:
        displayText("Day " + (i+1) + ": " + weeklyWeatherArray[i], x=100, y=150 + i*20)
    // Display average temperature
    displayText("Average Temperature: " + averageTemperature, x=100, y=300)
    // Display button for detailed daily views
    displayButton(button, x=100, y=350, onClick=displayDailyViews)
    // Display button to exit the app
    displayButton(button, x=100, y=400, onClick=exitApp)

// Function to calculate average temperature
FUNCTION calculateAverageTemperature():
    totalTemperature = 0
    FOR i FROM 0 TO 6:
        totalTemperature = totalTemperature + weeklyWeatherArray[i]
    averageTemperature = totalTemperature / 7

// Function to navigate to detailed daily views
FUNCTION displayDailyViews():
    // Implement navigation logic to the second screen for detailed daily views
    navigateToDailyViewsScreen()

// Function to exit the app
FUNCTION exitApp():
    // Implement exit logic to close the app
    closeApp()

// Main function
FUNCTION main():
    // Load images
    loadImages()
    // Fetch weekly weather data and populate array
    fetchWeeklyWeatherData()
    // Calculate average temperature
    calculateAverageTemperature()
    // Display splash screen UI
    displaySplashScreen()

// Call main function to start the app
main()
stop


Screenshots
 


 



 




GitHub repository
https://github.com/ST1044043/splashproject.git

PowerPoint presentation
https://advtechonline-my.sharepoint.com/personal/st10440433_vcconnect_edu_za/Documents/purpose.pptx?web=1
