## Notifications and Threads Review
Jared Poelman  

##### Previous lectures  
[Threading](https://github.com/accesscode-2-1/unit-2/blob/master/lessons/10_Threads.md)  
[Notifications](https://github.com/accesscode-2-1/unit-2/blob/master/lessons/11_Notifications.md)  

#### [Slides](21_Review_Thread&Notif_slides.pdf)

### Notifications

Design guide:
http://developer.android.com/design/patterns/notifications.html

API guide:
http://developer.android.com/guide/topics/ui/notifiers/notifications.html

NotificationCompat.Builder:
http://developer.android.com/reference/android/support/v4/app/NotificationCompat.Builder.html

Notification.Builder:
http://developer.android.com/reference/android/app/Notification.Builder.html

- Builder Pattern

- Notification UI

- Android SDK version gating

### Threads

Concurrency:
https://docs.oracle.com/javase/tutorial/essential/concurrency/index.html

- UI Thread

- Atomicity

- Shared Preferences

- Synchronized

### Exercises

1) Create a notification with an API level gated feature!

http://developer.android.com/reference/android/os/Build.html

2) Create a Builder class!

https://en.wikipedia.org/wiki/Builder_pattern#Java_Example

3) Challenge: Create a working example of deadlock!

https://en.wikipedia.org/wiki/Deadlock

4) Challenge: Create a notification that displays an image from a URL!

## Exit Ticket  
Please submit the exit ticket [here](https://docs.google.com/forms/d/1YlBu5qmGigbq5AdfiU4x-E7JVoDShq4lSacoetuu5ZA/viewform).  

### Exit Tickets Questions & Answers :-)
1.  What is a notification id?  
  The id used to identify a notification to the Android system.  It can be used to delete a notification.
  
2. How is the UI thread different from other threads on Android?   
  Android applications are single-threaded by default.  This thread is called the UI thread and manages all UI events.  Non visible long-running or blocking tasks (e.g. network, database I/O) should be run in separate threads to avoid blocking the UI thread.
  
3. Why would you use NotificationCompat instead of Notification?  
   To extend support for Notification API features to earlier API levels in backwards-compatible fashion
