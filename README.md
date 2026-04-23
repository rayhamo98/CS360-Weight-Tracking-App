# CS 360 - Mobile Architecture & Programming  
**Final Portfolio Artifact**

**Student Name:** Rimon Hamo  
**Date:** April 23, 2026

---

## Portfolio Artifact

**Project Three – Weight Tracking App**  
[Download Completed App ZIP](https://github.com/rayhamo98/CS360-Weight-Tracking-App/raw/main/Weight_Tracking_App_RimonHamo.zip)

This ZIP contains the full Android Studio project with all features implemented.

---

## Reflection Questions

### Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?

The Weight Tracking App was designed to help users monitor their weight loss or fitness journey. The main goals were to allow users to create an account, securely log in, record daily weight entries (with date and unit selection - kg or lbs), view their complete history, set a personal goal weight, and receive an SMS notification when they reach their goal. 

It addresses key user needs such as simplicity, data persistence, progress tracking, and motivation through goal achievement alerts.

### What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?

I created five main screens:
- Login / Register
- Dashboard (welcome + quick navigation)
- History (RecyclerView list of all entries)
- Add Weight (dialog)
- SMS Permission settings

The UI was kept clean and simple with large buttons, clear labels, and consistent colors. I used RecyclerView for easy scrolling through history and made sure important actions (Add Weight, View History) were always visible. The design is user-centered because it focuses on quick data entry and clear progress visibility — users can log weight in just a few taps.

### How did you approach the process of coding your app? What techniques or strategies did you use? How could those techniques or strategies be applied in the future?

I followed a modular and iterative approach:
1. Set up SQLite database and user authentication first
2. Built the login/register system
3. Created the Dashboard and navigation
4. Implemented the History screen with RecyclerView + Adapter
5. Added goal setting and SMS functionality last

I used separation of concerns (separate classes for DatabaseHelper, Activities, Adapter) and tested each feature individually before connecting them. This strategy helped me catch bugs early and made the code much easier to maintain. I will definitely use this step-by-step modular approach in all future app development projects.

### How did you test to ensure your code was functional? Why is this process important, and what did it reveal?

I performed extensive testing using the Android Emulator:
- Manual testing of all user flows (register, login, add weight, delete, unit switching)
- Edge cases (empty fields, invalid input, permission denied)
- Persistence testing (close and reopen app to verify data remains)
- SMS functionality testing

Testing was crucial because it revealed bugs in RecyclerView refreshing, unit conversion logic, and permission handling that I was able to fix before submission. It gave me confidence that the app is stable and user-friendly.

### Consider the full app design and development process from initial planning to finalization. Where did you have to innovate to overcome a challenge?

The biggest challenge was connecting everything together — especially refreshing the RecyclerView after adding or deleting entries and handling kg/lbs conversion properly. I had to innovate by creating a custom `WeightEntry` inner class and improving the adapter’s `updateData()` method. Another challenge was SMS permission handling — I created a dedicated settings screen with a toggle so users can enable/disable notifications.

### In what specific component of your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?

I am most proud of the **History screen with RecyclerView + Adapter** and the **SQLite integration**. Being able to display dynamic data from the database, support delete functionality, and handle unit conversion shows strong understanding of Android architecture, adapters, and database management — skills I can confidently discuss in job interviews.

---

**Thank you for reviewing my CS 360 Portfolio Artifact!**

---

### What to Do Now:
1. Go to your GitHub repo → Edit `README.md`
2. Paste the entire text above
3. Update the ZIP download link if needed
4. Submit the repository link in your course

Would you like me to make any part longer, shorter, or more personal? Just say the word and I’ll adjust it immediately. 

You’re done with CS 360! 🎉
