AIM

Create an Android Application to demonstrate Frame-by-frame animation and a splash screen to demonstrate tween animation.

Concepts to Study
ImageView
Frame-by-Frame Animation
Tween Animation
Immersive Mode
Display Edge to Edge
SplashScreen
AnimationDrawable
onWindowFocusChanged() Method
AnimationUtils class
loadAnimation() method
setAnimationListener() method
overridePendingTransition() method
finish() method
anim folder in res
Convert SVG file to .xml file
Theory
What is Frame by Frame Animation?
Frame-by-frame animation is an animation technique where each frame is drawn individually. It's like a flipbook. When you show the drawings in quick succession, it creates the illusion of movement. In Android, this is typically implemented using the AnimationDrawable class, where a sequence of drawable resources is defined in an XML file (usually in res/drawable) using the <animation-list> element.

What is Tween Animation?
Tween (short for in-between) animation is a type of animation where you define the start and end points of an animation, and the system creates the intermediate frames for you. It's used to perform transformations on a View, such as changing its position, size, rotation, and transparency. In Android, tween animations can be defined in XML files (in the res/anim folder) using tags like <scale>, <translate>, <rotate>, and <alpha>, all grouped within a <set> tag.

How can you achieve edge-to-edge content display in your app?
To achieve an edge-to-edge display, allowing your app to draw behind the system status and navigation bars, you should use the WindowCompat.setDecorFitsSystemWindows(window, false) method, typically in your Activity's onCreate method. This tells the system that your app's views will handle fitting the content within the system windows. You might then need to adjust your layout's padding or margins to prevent important UI elements from being obscured by the system bars.

Application Instructions
SplashActivity
Create a SplashActivity that shows a logo with a tween animation.
The animation should use a combination of <scale>, <translate>, <rotate>, and <alpha> tags.
After the animation, navigate to MainActivity.
MainActivity
Design the layout for MainActivity as shown in the provided screenshot.
Implement a frame-by-frame animation on the ImageView to cycle through different images of an alarm clock.
Use an <animation-list> in a drawable resource for the frame-by-frame animation.
Screenshots
![image alt]()
