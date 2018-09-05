# Android Interview Preparation

A collection of materials, interview questions with answers, Android tips, best practices specially for Android interviews.

## Interview Questions

### Data Storage And Access
* [How to access data in Content Providers?](#cp1)

dfdfdf

s
df

sd
f
s
d
f
sd
f

sd
f
sd
f

sdf

sd
f
sd
#### A : Access data in Content Providers<a name="#cp1"></a>
Start by making sure your Android application has the necessary read access permissions. Then, get access to the ContentResolver object by calling getContentResolver() on the Context object, and retrieving the data by constructing a query using ContentResolver.query().

The **ContentResolver.query()** method returns a Cursor, so you can retrieve data from each column using Cursor methods.

### References
https://android.jlelse.eu/android-interview-questions-cheat-sheet-96ea01c88def<br>
https://android.jlelse.eu/android-interview-questions-cheat-sheet-part-ii-bea0633f0da7
