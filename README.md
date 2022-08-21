<img src="https://spaghetcodes.best/img/virtual-hypixel/VirtualHypixelBanner.png">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Oxanium&display=swap" rel="stylesheet">

<h2 align="center" style="font-family: 'Oxanium', cursive;">
   What is Virtual Hycraft?
</h2>

Virtual Hycraft is a tool that improves your gameplay on Hycraft! It comes packed with many
features that make your life easier, including a stats mod, and fps booster (kind of) and more.

<br>
<details>
  <summary>Fork Information</summary>
  <p>Virtual Hycraft is just a fork of Virtual-Hypixel-v4 (https://github.com/HumanDuck23/virtual-hypixel-v4) with the server changed to support Hycraft instead of Hypixel, all of the code credit goes to the creator of Virtual Hypixel, Sphaget aka HumanDuck23. Some modifications have been made for Hycraft Support, but 99% of the code is by him or based from his code. So please check out and star his repository if you use this <3</p>
</details>

<h2 align="center" style="font-family: 'Oxanium', cursive;">
   Features
</h2>

<details>
  <summary>Pre-Game Stats</summary>
  <p>Virtual Hycraft shows the stats of your opponents before the game starts (including duels, after the update).</p>
</details>
<br>
<details>
  <summary>AutoGG</summary>
  <p>With most proxies like this AutoGG and other Hycraft mods don't work, so Virtual Hycraft implements its own AutoGG.</p>
</details>
<br>
<details>
  <summary>Better Ping</summary>
  <p>The Better Ping module updates your ping more frequently in-game and counteracts the problem of the ping mod showing 1ms. </p>
</details>
<br>
<details>
  <summary>Custom Commands</summary>
  <p>Virtual Hycraft implements a few custom commands, such as the <code>/sc</code> command for stat checking and <code>/rq</code> to quickly requeue your current (or last) game.</p>
</details>
<br>
<details>
  <summary><code>/play</code> Protection</summary>
  <p>Have you ever accidentally run <code>/play</code> while in game? Virtual Hycraft will ask you to confirm the command to avoid leaving the game.</p>
</details>
<br>
<details>
  <summary>Basic FPS Boost</summary>
  <p>The FPS Boosting module can filter out a few things sent by Hycraft to improve FPS.</p>
</details>
<br>
<details>
  <summary>Settings (WIP)</summary>
  <p>Virtual Hycraft allows you to change settings in-game with a nice and simple settings window.</p>
</details>


<h2 align="center" style="font-family: 'Oxanium', cursive;">
   How do I use it and set it up?
</h2>

Since there is no release yet, you'll have to do a lot of the work yourself to get this running. Here are the steps:

*You'll need to have [NodeJS](https://nodejs.org/) and [TypeScript](https://www.typescriptlang.org/download)
installed.*

**Make sure you have NodeJS and TypeScript installed, links are above**
1. Download this repo as a ZIP
2. Extract the ZIP file you just downloaded
3. Open CMD (click Search in your task bar and then type "cmd") and use the command below to change directories into the folder you extracted it to
   a. `cd (your folder location, ex. C:\Users\jos\Downloads\virtual-hycraft-v4-master\virtual-hycraft-v4-master`
4. Once your in the directory, install the dependencies by running the command `npm i`
5. Fill out the config file (config.yaml) in the installation directory's src folder (ex. `src/config.yaml`)
6. Rename `config.yaml` to `config_priv.yaml` once you're finished filling it out
7. Create a file in src: `app.ts`
  a. Make sure to open this file in Notepad once it's made, ignore the file extension warning, just make the file extension is .ts and the name is app (app.ts)
8. Paste this code in the file whilst in notepad, then save:
    ```ts
   import { VirtualHypixel } from "./proxy/classes/VirtualHypixel"
    const vh = new VirtualHypixel("./config_priv.yaml")
    vh.start()
    ```
9. Compile all the TypeScript code by typing `tsc` or `npx tsc` in CMD (run the other command if one does not work)
10. Run `app.js` with `node app.js`
