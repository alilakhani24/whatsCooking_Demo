# whatsCooking_Demo
This is a demo video of my whatsCooking project. The code is in Java and made in Android Studio. Request for access!

## Status Report 

As of August 6th, 2021 the What’s Cookin app has reached a completed state. From the three original functional requirements we set out to complete, we have added an additional one that we believe will make the app more appealing to its users. A list of these requirements can be seen below with more detail:
1. Repeatedly display two restaurants and allow the user to pick a preferred restaurant
This functionality was implemented with the help of the Yelp Fusion API. The API allowed us to effectively retrieve a list of restaurants based on the user’s current latitude and longitude measurements. From this, we used the pipe and filter architecture to filter these results and display the restaurants in the form of card components. To make this functionality more intuitive for our users, we implemented it with swipe gestures and disabled button states. The playoff bracket simulation was chosen for gamification purposes and as an intuitive UI that resembles many sport leagues.
2. The system will filter restaurants based on different criteria provided by the user
We were able to implement this functionality through a series of different classes and the Yelp Fusion API. The filter logic for this was implemented as part of the request parameters in the API call and the data parsing performed after the restaurant list was retrieved. Filters include radius in metres, price level of the restaurants and a maximum number of comparisons.
3. Various statistics of the current restaurants such as ratings, food types, and distance from current location will be displayed during the game
We were able to implement this functionality using the data retrieved from the Yelp Fusion API. The JSON data from the API call provided us with several fields that we could use as statistics for the restaurant. Due to this, displaying these statistics simply required the data to be filtered properly and the component to be rendered correctly.
4. Users can earn badges while playing the game and these badges alongside a history of selected restaurants can be seen on their profile.
This was a requirement that we created after our initial proposal. We were able to implement this through our Data class which handled reading and writing to the device’s local storage. With the Data class in place, we simply needed to call these read and write functions at the end of the restaurant picker game and when the user entered their profile page. The intent of this function was to provide historical data and trends to users, while also serving as a visual to prevent prolonged or repetitive use to regenerate past results - thereby limiting addiction.
      
During development, we had to make the difficult decision to remove some functionality we listed in our initial proposal. This was due to certain challenges that we faced during development and a prioritization on our part to make sure the key functionalities were still going to be captured by the end. A list of these dropped functionalities can be seen below in detail:
1. Allowing the user to elect an early ending to the restaurant picker game
After discussing this among ourselves, we decided that it’s possible for users to still find value in continuing to play the game even if they have seen a restaurant that they like. We could
foresee users finding value in simply discovering more restaurants in their area or selecting another restaurant that they prefer over their current preference. Force restarting the app would innately allow for an early exit.
2. Accessibility non-functional requirements (WCAG, text-to-speech, colorblind mode) From our initial proposal, we stated that we wanted to satisfy certain accessibility requirements in order to reach as wide of a user base as we could. During development however, we decided that these requirements were not crucial to the application and our time was better spent focusing on completing and polishing the more important functional and non-functional requirements. We reached this conclusion after investigating the implementation of these accessibility requirements and discovering certain challenges that we would face. For the WCAG requirements we discovered that in order for us to be able to say that the app is WCAG 2 compliant, we would need to implement an extensive list of guidelines and as a result we decided that our time would be better off spent focusing on making the core functionalities of What’s Cookin work properly. In terms of the text-to-speech requirement, we faced a challenge configuring the settings and would have had to configure many functioning components.

## Demo Description

For our demo, we will be showcasing the What’s Cookin app in its final form. We have improved various UI components and added certain components to help us satisfy our desired functional and non-functional requirements. Notably, as a non-functional requirement, we implemented dark mode compatibility which changes the colour scheme upon changing the android device settings. The below demo run through will include technical underpinnings, selected design choices, and edge cases supported in the app as they appear in the run through.

## Users perspective:


- The demo will begin from the splash screen intended to welcome users to the application while data is loaded into the application to prevent delay frustrations
- The landing page features help and resource buttons in addition to gameplay and profile buttons that segway into their respective activities. As a new user, the help menu will be explored followed by the profile menu
- Profile will be changed according to the user’s identity and then transition to game play
- Game play will begin with the filter page to curate a customer restaurant playoff bracket.
- A mock game play will be played from the user’s perspective until the final results page.
- Upon completing the entire user interface, the demo will revisit the profile page to show
the now updated history and achievements list and pop-up capability.
- Dark mode will be explored, and data storage will be shown to demonstrate saving states


