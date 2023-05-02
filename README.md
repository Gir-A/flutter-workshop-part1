# Flutter Workshop Part 1
#### *by [Annaïg LEIZOUR](https://github.com/Gir-A) and [Bruno DE OLIVEIRA](https://github.com/n0no123)*

---

## Disclaimer
This workshop was made for VSCode user in mind. We'll provide you with a devcontainer configurations files, meaning that you won't need to go through the process of installing Flutter and the other dependencies. Should you wish to not use VSCode, please we are available to help you through the installation process.

## Step 0: Setting up your workspace

### Docker:
To use the provided devcontainer, you will need to have docker installed.

You can use a script to install Docker (provided by... Docker!) using the following command:

```shell
  curl -fsSL https://get.docker.com -o get-docker.sh
```
You can then run it using (you may need to set the correct permission beforehand):
```shell
  sudo sh get-docker.sh
```

If it doesn't work, or if you don't wish to use the script you can always install by following the instruction on [Docker website](https://docs.docker.com/engine/install/).

### VSCode:

You can install VSCode by following the instruction [here](https://code.visualstudio.com/download).

Clone the [repository](git@github.com:Gir-A/flutter-workshop-part1.git) and install the [VSCode Dev Containers Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers).

It should prompt you with a popup on the lower-right-side of your screen asking to open the folder in a container. If not, open the Command Pallette with <kbd>ctrl</kbd> + <kbd>⇧ shift</kbd> + <kbd>P</kbd>, and type **>Dev Containers: Open Folder in Container...**. You can now wait for a good 5-10 minutes (depending on the Wifi) while it builds your container and install all the necessary dependencies inside your container.

---

### Step 1: Create an empty project

Well, I say empty, but Flutter will create a small app for you that will implement a counter.

Create the project by running

```shell
  flutter create app_name
```

If you want to know more about the create command, just type:
```bash
  flutter help create
```
It should give you a ton of info you might never use but are still cool to know.

(It should be written on your terminal after you've created the project, but repeating never hurts.) You can use:
```bash
  flutter run
```
to see what this counter app is all about.

#### USB debugging & Developer mode

If you have never used your phone to develop an app, you should have an error when trying to run your app.

You will need to enable **Developer mode** (more information about that [here](https://www.xda-developers.com/android-developer-options/)) on your phone (just do a quick search on how to do it with your phone model). That should unlock a whole lot of new settings. Inside those settings you need to enable **USB Debugging** so that your computer may access your phone.

You will also need to **grant permission** when prompted on your phone and your phone should be in **file transfer mode** when connected to your computer.

You can run:
```shell
  flutter devices
```
in order to check that your phone is available to your app.

You can also run:
```shell
  flutter doctor
```
to check on your app's vitals. Kidding, but it still gives you basic info on your app and includes your available devices in its output.

You should now be able to run the app.

Once that's done and your app is running on your phone, just tell me so. I have a little presentation of the project structure for you guys.

---

### Step 3: Make a Home page and a Display page

https://docs.flutter.dev/development/ui/widgets-intro

Now that the basics are covered, let's start coding. 
[Here](https://docs.flutter.dev/cookbook/navigation/navigation-basics) is a link to get you started.

You can start coding everything in your main file in the lib folder OR you can create 2 files and code each page in each file. (**Second way is cleaner**) *If you need anything in a file from another, you can of course just import it.*

*Also, if you create new files, __please__ use snake_case convention for the file names. More information about that [here](https://dart.dev/guides/language/effective-dart/style).*

Once again, if you run into serious trouble on this step, we are available to answer any questions. But you shouldn't have too much trouble, *I believe in you!*

---

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
