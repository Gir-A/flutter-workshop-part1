# Flutter Workshop Part 1
###### *by Annaïg Leizour*

-------------------------------------
### Step 1: Do you have Docker installed?
<details>
<summary>Yes</summary>

##### Great!

You will be able to use a Dev Container for this workshop!

Open VSCode and install an extension called **Dev Containers**. Enable it if that's not done.

Clone the repo and open the folder with VSCode. It should show you a popup on your lower-right-side asking to open the folder in a container.
Click on it. You can now wait for a good 5-10 minutes (depending on the Wifi) while it builds your container and downloads flutter in it for you.

But once that's done, you can start coding in Dart!

</details>

<details>
<summary>No</summary>

##### What a bummer!
##### *You did not attend my Docker workshop, how unfortunate! You can now download flutter on your computer or download docker: __link_to_docker_install_or_workshop__ to be able to use a container*
### Installing flutter

https://docs.flutter.dev/get-started/install

Choose your distribution and follow the steps!

I am available if there are any problems

Nota Bene1:
You do not need Android Studio to use Flutter. If ``flutter doctor``returns a message saying Android SDK is missing you can download it using ``apt install android-sdk`` if you are on ubuntu.
Same goes for cmdline-tools. Just run ``sdkmanager --install "cmdline-tools;latest"`` You might have to write the whole path for sdkmanager. You can also download the cmdline-tools from https://goo.gl/XxQghQ. This should bring you to android studio's site just scroll down and select the zip file according to your distribution.

Nota Bene2:
It might be easier to just download Android Studio but it does take up a lot of space on your computer (especially if you use emulators).

</details>


---------------------------------------

### Step 2: Create an empty project

Well, I say empty, but Flutter will create a small app for you that will implement a counter.

Create the project by running ``flutter create name_of_your_app`` Use snakecase for your project name!

(It should be written on your terminal but) You can use ``flutter run`` to see what this app is all about.

Phone USB debugging & Developer mode

Once that's done and your app is running on your phone, just tell me so. I have a little presentation of the project structure for you guys.

---------------------------------------

Create an empty project - Explanation of what is what in the project structure, “where do I code?”

Make a home page (and route) and navigate to another route and back.

Make a few API calls to the API of their choice. - I will provide them with a list of easy to use APIs. (+ small API introduction: what is an API - use of external APIs)
Present a few interesting widgets to know.
