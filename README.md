# IMAD-EXAM
**Campsite Commander**
An Android application built with Kotlin, demonstrating the use of the app. it stores camping gears and food supplies, allowing the users to categorize them and it provides a detailed checklist view.

**Overview**
This project covers a designed app that was built with Kotlin using arrays, loops and screen navigation.

**Concepts Covered**
Toast messages — displaying short popup notifications using Toast.makeText()

Transition - transitioning to the next activity by declaring delayMillis

Error handling -  if (item.isEmpty() || category.isEmpty() ||

Log.d - Debug: Essential information for tracking variables or behavior

Layout structure — LinearLayout with TextView and Button in activity_main.xml

Setup
Clone the repository
Open in Android Studio
Let Gradle sync
Run on an emulator or physical device (Android 7.0)

class MainActivity : AppCompatActivity() {

    **Transition**

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)
           // 3000 milliseconds = 3 seconds
        val delayMillis = 3000L

        Handler(Looper.getMainLooper()).postDelayed({
// create intent to move to mainActivity
            val intent = Intent(this, MainActivity::class.java)
            startActivity(intent)

            finish()
        }, delayMillis)
    }
}

**Showing a Toast**

Toast.makeText(this, "Hello!", Toast.LENGTH_SHORT).show()

**Error Handling**
 // Error Handling
                if (item.isEmpty() || category.isEmpty() ||
                    quantityText.isEmpty() || comments.isEmpty()) {
**Log**
 }

                txtOutput.text = output

                Log.d("PACKING_APP", "Displayed quantity >= 2")
            }

Built With
Kotlin

Android SDK

AndroidX AppCompat
