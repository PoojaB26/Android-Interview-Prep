# Android Interview Preparation

A collection of materials, interview questions with answers, Android tips, best practices specially for Android interviews.

## Interview Questions

### Data Storage And Access
* [How to access data in Content Providers?](#cp1)
* [Content Values vs Cursor](#cp2)
* [Steps to create Content Provider](#cp3)

### Services
* [Difference between Service & Intent Service](#sc1)



#### <a name="cp3"></a> A : Steps to create Content Providers
1. Create a Table Contract
2. Setting up the DatabaseHelper
3. Setting up the Content Provider
4. Declare it on the manifest

#### <a name="cp1"></a> A : Access data in Content Providers
Start by making sure your Android application has the necessary read access permissions. Then, get access to the ContentResolver object by calling getContentResolver() on the Context object, and retrieving the data by constructing a query using ContentResolver.query().

The **ContentResolver.query()** method returns a Cursor, so you can retrieve data from each column using Cursor methods.

#### <a name="cp2"></a> A: Content Values vs Cursor
Content Values is a name value pair used to insert and update values into database tables. Content Value objects will be passed to SQLiteDatabase object's insert or update function. 

Cursor is a temp buffer which stores results from the SQLiteDatabase

#### <a name="sc1"></a> Difference between Service & Intent Service
Service is the base class for Android services that can be extended to create any service. A class that directly extends Service runs on the main thread so it will block the UI (if there is one) and should therefore either be used only for short tasks or should make use of other threads for longer tasks.
IntentService is a subclass of Service that handles asynchronous requests (expressed as “Intents”) on demand. Clients send requests through startService(Intent) calls. The service is started as needed, handles each Intent in turn using a worker thread, and stops itself when it runs out of work.

### References
https://android.jlelse.eu/android-interview-questions-cheat-sheet-96ea01c88def<br>
https://android.jlelse.eu/android-interview-questions-cheat-sheet-part-ii-bea0633f0da7
http://skillgun.com/android/content-providers/interview-questions-and-answers/paper/28
