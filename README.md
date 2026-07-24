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
Program to print the text “Hello World”.
Developed by: Dharunyadevi S
Registeration Number : 212223220018

```

MainActivity.java

```java
package com.example.lifecyclemethods;

import android.os.Bundle;
import android.widget.Toast;


import androidx.appcompat.app.AppCompatActivity;


public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast t = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onStart(){
        super.onStart();
        Toast t  = Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG);
        t.show();
    }
    @Override
    protected void onPause(){
        super.onPause();
        Toast t = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onResume(){
        super.onResume();
        Toast t = Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onStop(){
        super.onStop();
        Toast t = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onRestart(){
        super.onRestart();
        Toast t = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onDestroy(){
        super.onDestroy();
        Toast t = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        t.show();
    }
}



```

activity_main.xml

```xml
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>

```

## OUTPUT

#### 1.onCreate:

<img width="1920" height="1080" alt="Screenshot (330)" src="https://github.com/user-attachments/assets/2596db9b-6d17-40e9-987a-a17420639ed6" />

#### 2.onStart:
<img width="1920" height="1080" alt="Screenshot (328)" src="https://github.com/user-attachments/assets/970546cd-30af-42b2-9262-52829a30d080" />


#### 3.onPause:

<img width="1920" height="1080" alt="Screenshot (327)" src="https://github.com/user-attachments/assets/d0a549f3-9e81-48fd-99db-4b37bf4a6e7a" />

#### 4.onResume:

<img width="1920" height="1080" alt="Screenshot (332)" src="https://github.com/user-attachments/assets/108eec44-e9f9-4af2-867e-0f32392763ed" />

#### 5.onRestart:

<img width="1920" height="1080" alt="Screenshot (337)" src="https://github.com/user-attachments/assets/acd20ea2-2094-4146-ba28-3aacc5002835" />












## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
