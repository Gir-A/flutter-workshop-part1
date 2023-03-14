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

*Nota Bene 1:*

You do not need Android Studio to use Flutter. If ``flutter doctor``returns a message saying Android SDK is missing you can download it using ``apt install android-sdk`` if you are on ubuntu.
Same goes for cmdline-tools. Just run ``sdkmanager --install "cmdline-tools;latest"`` You might have to write the whole path for sdkmanager. You can also download the cmdline-tools from https://goo.gl/XxQghQ. This should bring you to android studio's site just scroll down and select the zip file according to your distribution.

*Nota Bene 2:*

It might be easier to just download Android Studio but it does take up a lot of space on your computer (especially if you use emulators).

</details>


---------------------------------------

### Step 2: Create an empty project

Well, I say empty, but Flutter will create a small app for you that will implement a counter.

Create the project by running ``flutter create name_of_your_app`` Use snakecase for your project name!
You can also give your actual folder's path like so ``flutter create ..\simple_app`` (if you're using the Dev Container). It should create every file necessary in your actual directory whereas the other command would create another directory with the files inside of your current folder.

If you want to know more about the create command, just type ``flutter create`` it should give you a ton of info you might never use but is still cool to know.

(It should be written on your terminal after you've created the project, but it never hurts to repeat.) You can use ``flutter run`` to see what this counter app is all about.

#### USB debugging & Developer mode

If you have never used your phone to develop an app, you should have an error when trying to run your app.

You will need to enable **Developer mode** on your phone (just do a quick search on how to do it with your phone model). That should unblock a whole lot of new settings. Inside those settings you need to enable **USB Debugging** so that your computer may access your phone.

You will also need to **grant permission** when prompted on your phone and your phone should be in **file transfer mode** when connected to your computer.

You can run ``flutter devices`` in order to check that your phone is available to your app.

You can also run ``flutter doctor`` to check on your app's vitals. Kidding, but it still gives you basic info on your app and includes your available devices in its output.

You should now be able to run the app.

Once that's done and your app is running on your phone, just tell me so. I have a little presentation of the project structure for you guys.

---------------------------------------

### Step 3: Make a Home page and a Display page

https://docs.flutter.dev/development/ui/widgets-intro

Now that the basics are covered, let's start coding. 
[Here](https://docs.flutter.dev/cookbook/navigation/navigation-basics) is a link to get you started.

You can start coding everything in your main file in the lib folder OR you can create 2 files and code each page in each file. (**Second way is cleaner**) *If you need anything in a file from another, you can of course just import it.*

*Also, if you create new files, __please__ use snake_case convention for the file names.*

Once again, if you run into serious trouble on this step, I am available to answer any questions. But you shouldn't have too much trouble, *I believe in you!*

---------------------------------------

### Step 4: Make a few API calls

Wait a minute! Do you know what an API is and how it works?

If you do, then you can go on and continue this workshop. If not, please inform me that you have reached step 4. Once again, I have prepared a little introduction for you guys.

Here are a few APIs you can use for this step. The documentation is pretty explicit and easy to use.
 - [Official Joke API](https://github.com/15Dkatz/official_joke_api)
 - [PokeAPI](https://pokeapi.co/)
 - [OpenWeather](https://openweathermap.org/)
 - [TriviaAPI](https://opentdb.com/api_config.php)
 
 Just choose one (or multiple if you're feeling a bit daring!) and start making some calls. Get started using [this](https://docs.flutter.dev/cookbook/networking/fetch-data)

### *To Go Further:*
 
  You can find other cool APIs (which I have not tested) on [here](https://github.com/public-apis/public-apis#index)
It can also help you find ideas for other workshops or even talks if there is an API that you find fantastic and cannot wait to talk about!

  You may find that we haven't covered much in this workshop (I agree). If so, here is a list of widgets that you might find interesting:
  - [Drawer](https://api.flutter.dev/flutter/material/Drawer-class.html)
  - [Navbar](https://api.flutter.dev/flutter/material/NavigationBar-class.html)

  Also, the flutter links we have used for API calls and navigation between routes are part of the Flutter **[CookBook](https://docs.flutter.dev/cookbook)**. So, check that out, it's a really great startpoint to learning flutter.
  
  *Happy Fluttering!*
