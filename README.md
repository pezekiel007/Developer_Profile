# Developer_Profile
This is an app that shows the contact details of a developer.

The app shows the use of common views and the Linear Layout view group.

DEVELOPER PROFILE IMPLEMENTATION
================================

The following are steps to build the developer profile app:

1. Get Resources:
    This is the first stage of the process of building right after creating the project; The list of resources the app needs are as follows:
    - Image: A display picture of you, more like a headshot. This should be in the drawable package in the res folder.
    - Icons: An email and a phone icon; give them colours as well. These should be in the drawable package in the res folder.
    - Color: Make a color resource (grey colour), call it grey. This should be in the colors.xml file in the values package in the res folder.
    - Font: This is for your name as in the UI design given. This should be in the font package in the res folder.
    - Texts: Your name; Your tech course; Your phone number; Your email. This should be in the styles.xml file, in the values package in the res folder.

2. Build Layout:
    At this stage, we build the app (just the layout since there is no need for business logic at this point).
    - Open the activity_main.xml and Remove or Delete all views in the Constraint layout.
    - Change the Constraint Layout to a Linear Layout. ( The views in the UI design are vartically aligned and the Linear Layout will make it easy to implement it)
    - Give the Linear Layout the following attributes:
          * android:background="@color/teal_700": Choose any color from the color resource
          * android:gravity="center": To centralize the views on the layout. (Centered horizontally and vertically)
          * android:orientation="vertical": This tell the views to be arranged from top to bottom.
          * android:padding="16dp": Gives 16dp worth of space between the Linear Layout and the views.
    
    - Bring in a CardView.
    - Change the values of the layout_width and layout_height to 120dp.
    - Add these attributes:
          * android:backgroundTint="@color/teal_200": Choose any color from the color resource. (The background attribute doesn't change the colour)
          * app:cardCornerRadius="100dp": This will turn the square looking cardview to a circle to fit the given UI design.
    
    - Bring in an ImageView and put it in the Card View.
    - The source image to select is the display image of yourself you in the drawable package.
    - Set a contentDescription attribute, to which the value should be a description of the image. (Description should be short and do not forget to extract string resource.

    - Bring in a TextView. (This will serve for your name displayed with the stylish font)
    - Give the TextView the following attributes:
          * android:fontFamily="@font/pacifico_regular": This is the desired font as in the UI design.
          * android:text="@string/full_name": The text should be your name that is already saved in the strings.xml file.
          * android:textAlignment="center". This aligns the text to the center
          * android:textColor="@color/black": Choose any color and the colour should be visible.
          * android:textSize="30sp"
          * android:textStyle="bold"

    - Bring in another TextView. (This will serve for your tech course)
    - Give the TextView the following attributes:
          * android:text="@string/tech_course": The tech course saved in the strings.xml file.
          * android:letterSpacing="0.15": For spacing in between the letters.
          * android:textAlignment="center"
          * android:textColor="@color/black"
          * android:textSize="20sp"

    - Bring in a View. (Search for view in the pallete on Design interface)
    - Change the values of the layout_width to 150dp and layout_height to 1dp.
    - Give the View the following attributes:
          * android:layout_marginTop="8dp"
          * android:background="@color/black": Choose any color and the colour should be visible.

    - Open your project folder (if closed), right-click on the drawable package, click on new, click on drawable resource file.
    - Type in "grey_bg" as the name and click OK.
    - In the grey_bg file, change the selector to shape and give an attribute called shape with rectangle as a value.
    - In between the shape start and end tag, add the following:
          * <solid android:color="@color/grey"/>
          * <corners android:radius="5dp"/>

    - Bring in a TextView. (This will serve for your phone number and email)
    - Give it the following attributes:
          * android:layout_marginTop="16dp": For space between and the view above it.
          * android:background="@drawable/grey_bg": The drawable resource file called grey_bg will be the background.
          * android:drawablePadding="20dp": Space between the icon inside the textview and the text.
          * android:padding="20dp": Space between the border of the textview and the elements inside of it.
          * android:text="@string/phone_number": The phone number saved in the strings.xml file
          * android:textColor="@color/teal_700"
          * android:textSize="22sp"
          * android:textStyle="bold"
          * app:drawableStartCompat="@drawable/ic_call": The call icon at the start position of the textview.

    - Between Code, Split and Design towards the top-right of the IDE, click on Design to select it.
    - On the design surface, click on the TextView for the phone number.
    - After you have clicked on it; At the bottom-left, underneath the Component Tree, you will see the TextView highlighted grey.
    - Click on it from the component tree. (The textView will be highlighted blue at this point)
    - Press CRTL + C (to copy) and CTRL + V (to paste).
    - You should have two exact TextViews with the same phone numbers and the grey background.

    - On the second TextView, change the value of the app:drawableStartCompat the ic_email icon, also
    - Also, change the text attribute to your email. (The saved email in the strings.xml)

3. Remove Appbar of Toolbar:
    - Open your project folder. (If project folder is closed)
    - Click and Open the res folder.
    - Click and Open the values directory.
    - Under the values directory, click and open the themes directory then open the themes.xml file.
    - In the themes.xml file, in the parent attribute of the Style start tag; Change "DarkActionBar" to "NoActionBar" and leave every other thing the way it is.

4. Full Screen App.
    - Still in the themes.xml.
    - Click at the end of this (<!-- Customize your theme here. -->) comment and press your enter key.
    - Add an item tag (Less than sign and type item).
    - Add a name attribute to this tag and give it a value of "android:windowFullscreen".
    - Close the tag with this ">"; This should give a closing tag automatically.
    - Between the start tag and the end tag type true.
    - At the end you should have this: <item name="android:windowFullscreen">true</item>

The above steps (if followed) should help you develop or design this app on your own.

Thanks for using this resource...
