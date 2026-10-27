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
/*
Program to print the text “Hello World”.
Developed by:VAZHIGA BANU S 
Registeration Number :212225040484
*/
```
MAINACTIVITY.JAVA
```

package com.example.test;

import android.os.Bundle;
import android.widget.Toast;

import androidx.activity.EdgeToEdge;
import androidx.appcompat.app.AppCompatActivity;
import androidx.core.graphics.Insets;
import androidx.core.view.ViewCompat;
import androidx.core.view.WindowInsetsCompat;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast t = Toast.makeText(getApplicationContext(),"onCreate Called", Toast.LENGTH_LONG);
        t.show();

    }
    protected void onStart(){
        super.onStart();
        Toast t = Toast.makeText(getApplicationContext(),"onStart Called", Toast.LENGTH_LONG);
        t.show();
    }
    protected void onRestart(){
        super.onRestart();
        Toast t = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        t.show();
    }
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
    protected void onDestroy(){
        super.onDestroy();
        Toast t = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        t.show();
    }


}
```

ACTIVITY_MAIN.XML

```

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="WelcometoAndroidStudio"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>


```


## OUTPUT
onCreate()

<img width="1917" height="1190" alt="Screenshot 2026-10-27 114202" src="https://github.com/user-attachments/assets/2d3a9246-6808-430d-9ce7-0166804a7688" />



onStart()

<img width="1917" height="1192" alt="Screenshot 2026-10-27 114225" src="https://github.com/user-attachments/assets/eedc0c18-340c-478c-8c52-8170d8ee2ce8" />



onPause()

<img width="1917" height="1192" alt="Screenshot 2026-10-27 114307" src="https://github.com/user-attachments/assets/382b7dbd-528e-4480-a2b9-80a7d53f6a41" />



onResume()

<img width="1916" height="1190" alt="Screenshot 2026-10-27 114208" src="https://github.com/user-attachments/assets/839ce285-205b-486b-ac52-285501403409" />



activity_main.xml

<img width="1917" height="1195" alt="Screenshot 2026-10-27 100824" src="https://github.com/user-attachments/assets/7b22e384-9a5b-48bb-8ef2-29514be81c4f" />


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
