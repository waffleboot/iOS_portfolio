
# Finance Control app

It's an application for inserting expenses by clients and it has backend part on server and two mobile applications on iOS and Android, I worked as contractor for improving iOS application and implementing new features. First my task was adding iOS widget for fast insering of expenses because old application ran synchronization with backend on every appearing of application and people complained that it took too much time for sync by mobile network when they ran application right after shopping. So first my task was implementing widget for fast inserting information about expenses. I wrote widget (it looks like calculator) and it has most used expense items when you can write amount and choose the expense you had done. I wrote finete-state maching algorithm for correct processing of user input to create valid amount, wrote XCTests for all cases and optimized it and unit tests were very helpful for code coverage.

The application has outdated source code so I was needed to learn Obj-C to understand how it works. I worked with Core Data to understand how internal storage of application works, with network level of application (they don't use AFNet of something) for next task when I impelemented sending data over SOAP after parsing QR-code from cheque, fixed deadlock issue, tried to use Realm for storing data from widget but Realm stucks when it is used with their network level implementation. Made synchronization on moving app to background state because clients had complained about slow synchronization on appearing on slow mobile networks.

### Widget for "Finance Control" application

![Widget](https://github.com/waffleboot/iOS_portfolio/blob/master/images/image1.PNG)

### Main screen of "Finance Control application"

![Main Screen](https://github.com/waffleboot/iOS_portfolio/blob/master/images/image2.PNG)

### Closed tasks for "Finance Control application"

![Closed tasks](https://github.com/waffleboot/iOS_portfolio/blob/master/images/image3.PNG)

# wikipedia-iOS official app

Also I contributed a small code changes to official wikipedia-iOS application and it's very interesting how their application works on WKWebView (they have internal web server inside application and translates html from official site to internal presentation), I fixed CSS issues, investigated how it works but I wanted to implement video playing inside application because they cannot use proprietary AV codecs (as it open source) so I took OGVKit open source lib for media playing and tried to run video items from official site inside application. It works and I have send PR to him.

This is issue ticket https://phabricator.wikimedia.org/T68722

And this is proof of concept https://www.youtube.com/watch?v=rTb9peS9X6c

*So I can say that I have deep knowledge in UIKit (VC,CollectionViews,Tables),Core Animation (CALayers,implicit/explicit animations), Core Data (managed contexts in different dispatch queues,migration) but probably I need a some time to understand how to work with MapKit,AV for example.*

# and a couple of contribution to open source community

Dash (API Documentation Browser), Carthage

![Widget](https://github.com/waffleboot/iOS_portfolio/blob/master/images/image4.PNG)
