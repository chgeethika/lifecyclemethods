# Ex.No:2 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
Developed by:ch.geethika
Registeration Number : 212221040032
```
```
activity_main.xml

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:fontFamily="sans-serif-medium"
        android:text="Hello World!"
        android:textColor="#FF2256"
        android:textSize="34sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
```
MainActivity.java

package com.example.lifecyclesofandroid;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.Toast;
public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart() {
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG);
        toast.show();
    }
    @Override

    protected void onRestart() {
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onPause() {
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onResume(){
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onStop() {
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onDestroy() {
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();

    }
}
```
## OUTPUT
![Screenshot (295)](https://github.com/chgeethika/lifecyclemethods/assets/142209368/3ddf0fe8-e6ff-4a8b-88f2-88d3b996ee5b)
![Screenshot (296)](https://github.com/chgeethika/lifecyclemethods/assets/142209368/3d5c06a0-a8cd-4847-a9e8-e195f77b24b7)
![Screenshot (297)](https://github.com/chgeethika/lifecyclemethods/assets/142209368/79403547-1666-459f-b65f-b7336345c86f)
![Screenshot (298)](https://github.com/chgeethika/lifecyclemethods/assets/142209368/0b516caf-f14f-4d8b-80e5-1c48be1591d0)
![Screenshot (299)](https://github.com/chgeethika/lifecyclemethods/assets/142209368/9a3b9830-490d-4953-bbef-3c0cc8ac81c5)
![Screenshot (300)](https://github.com/chgeethika/lifecyclemethods/assets/142209368/53fe7a59-2971-4ac8-94fc-16e6a68a13aa)
![Screenshot (302)](https://github.com/chgeethika/lifecyclemethods/assets/142209368/f46bf606-b540-4083-82f8-a438c540ea75)

## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
