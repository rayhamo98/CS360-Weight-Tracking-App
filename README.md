# Project – Weight Tracking App

This project is a mobile application developed for CS 360 that allows users to track their weight over time. The app includes user authentication, daily weight logging with unit conversion (kg/lbs), history tracking, goal setting, and SMS notifications when goals are reached.

## Reflection

I developed the Weight Tracking App to support users in monitoring their weight loss or fitness journey. The main objectives were to enable users to create accounts, securely log in, record daily weight entries with date and unit selection, view their complete history, set personal goal weights, and receive SMS alerts upon reaching their goals. The app was designed with simplicity and motivation in mind to help users stay consistent with their progress.

The application consists of five primary screens: Login/Register, Dashboard, History (powered by RecyclerView), Add Weight dialog, and SMS Permission settings. I focused on creating a clean, user-centered interface with large buttons, clear labels, and consistent styling. The RecyclerView in the History screen allows users to easily scroll through past entries, while key actions like adding weight remain prominently visible. This design approach ensures quick data entry and clear visibility of progress with minimal effort from the user.

I began development by first creating the layouts and button structures, then progressively added functionality. I followed a step-by-step approach, starting with the user interface and navigation, followed by the login and registration system, Dashboard, History screen with RecyclerView, and finally the goal-setting and SMS notification features. I maintained clean code organization by separating concerns into distinct classes for the database, activities, and adapter. This methodical process helped me identify and resolve issues early while allowing me to see the application take shape incrementally.

To ensure functionality, I conducted extensive testing using the Android Emulator. I verified all user flows including registration, login, adding and deleting weight entries, unit switching, and SMS notifications. Edge cases such as empty fields and denied permissions were also tested. This process revealed issues with RecyclerView data refreshing and unit conversion logic, which were resolved prior to submission. Thorough testing was essential to confirm the app’s stability and reliability for end users.

One of the main challenges during development was ensuring the RecyclerView updated correctly after adding or deleting entries and implementing accurate kg/lbs conversion. I addressed these by creating a custom `WeightEntry` class and enhancing the adapter’s `updateData()` method. Additionally, I introduced a dedicated settings screen with a toggle switch to give users easy control over SMS notifications.

I am particularly proud of the **History screen with RecyclerView and Adapter**, along with the **SQLite database integration**. Successfully displaying dynamic data from the database, supporting delete functionality, and managing unit conversion demonstrates a solid understanding of Android architecture, adapters, and local data management — skills I can confidently apply in future development work and professional settings.

All code and content in this project were created by me. I only used basic spell-checking and grammar tools while preparing this README.
