# ChoreSpell
A random chore app (in progress).

Because sometimes it's easier just to do something random when you have a spare 5 minutes or half an hour or you just don't know where to start! At least, for those of us with questionable executive function.

**This app is actually a website that acts like an app.** It stores all your chores in local storage on your device, and doesn't keep stats or anything like that -- no login required -- so it's totally private!

## To install

Go to [the app](https://litlnemo.github.io/chorespell-pwa/) in a browser on your device. Tap the Share icon (on iOS) or the three dots in the top right corner of your browser window (on Android). Then choose "Add to Home Screen" (you might have to scroll down to find it). It will then put the "app" on your home screen and you won't have to go through a browser to use it!

## To use

Once you've installed it on your device, open the app and click the Random Chore button. It will show you a random chore. **Note:** If you haven't yet added your own chores, you will get one of three demo chores!

### Adding your own chores

There are two ways to add your own chores. 

- To add a single chore, use the Add Chores page. Click on the Add Chores link in the menu in the upper left of each page.

![Add Chores page](/readmepics/newchore.png)

- To add multiple chores, the chores need to be saved as JSON or CSV, as follows:

    JSON
```
    [
      {
        "name": "Make sure pictures are hanging straight",
        "category": "small",
        "image": ""
      },
      {
        "name": "Sweep bathroom",
        "category": "small",
        "image": ""
      }
    ]
```

  Just leave the "image" value empty. The "category" is referring to how big the chore is.

  CSV
```
Take trash to can ,Small,
Fluff couch cushions ,Small,
Quick trash pickup in living room ,Small,
Break down cardboard boxes,Large,
```
  
  - Go to the Backup and Restore page link in the menu in the upper left of each page.
  - Scroll down to the Import Chores section.
  - Note the checkbox labeled "Merge with existing chores (instead of replacing)?" If you already have chores in your app, you **MUST** check this box to keep them, otherwise the new chores will overwrite the old ones.
  - Paste your JSON or CSV data into the appropriate field.
  - Click the Import Chores button.
  - That's all!

### Editing existing chores

Click the View All Chores button in the menu on the upper left. You'll see a list of chores. Each has a pencil icon. Click the pencil icon to get into editing mode.

### Deleting existing chores

There is currently no delete button, but it's coming soon! In the meantime, you can edit the chore to be a different chore, or , more dangerously, backup your chores to JSON, delete the one you don't want, and import the JSON back in _without_ clicking the merge button. This will delete your entire chore list and re-import it, so be careful!

### Backing up and restoring your chore list

- Go to the Backup and Restore page link in the menu in the upper left of each page.
- Under **Export Chores**, select Show JSON.
- Now you have two options:
  - You can copy/paste the JSON text into a text file, and save it.
  - You can click the Download JSON button and it will generate the text file for you.
- To restore, go to the Backup and Restore page, and scroll down to Import Chores.
- Paste the text from your saved JSON file into the From JSON field.
- Click the Import Chores (JSON) button.

### Settings

Currently there is only one setting: Dark Mode. Select this to use the app in a less bright mode. 

## Warning

It's good to use the backup feature regularly, just in case! As long as you don't delete the app from your home screen and then re-add it, or overwrite them by forgetting to check the checkbox, your chores should stay intact -- but to be safe, if you have a lot of chores, it's best to back them up. Because typing all of them again would suck.
