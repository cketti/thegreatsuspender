# The Great Suspender

<img src="/src/img/suspendy-guy.png" width="100px" />

"The Great Suspender" is a Google Chrome extension that will automatically *suspend* tabs that have not been used for a while, freeing up memory and CPU cycles that the tab was consuming.

This is a fork of [greatsuspender/thegreatsuspender](https://github.com/greatsuspender/thegreatsuspender). It was created after the original project was suspected to contain malware; see https://www.theregister.com/2021/01/07/great_suspender_malware/.

Check out [CHANGELOG.md](CHANGELOG.md) for a list of changes in this fork.

### Not maintained!

I currently have no intention of maintaining this extension for anyone but myself. You're very welcome to fork this repository. But please don't contact me with feature requests or about errors.

### Install as an extension from source

1. Download the **[latest available version](https://github.com/cketti/thegreatsuspender/releases)** and unarchive to your preferred location (whichever suits you).
2. Using **Google Chrome** browser, navigate to chrome://extensions/ and enable "Developer mode" in the upper right corner.
3. Click on the <kbd>Load unpacked extension...</kbd> button.
4. Browse to the src directory of the unarchived folder and confirm.

If you have completed the above steps, the "welcome" page will open indicating successful installation of the extension.

Be sure to unsuspend all suspended tabs before removing any other version of the extension or they will disappear forever!

### Build from github

Dependencies: openssl, npm.

Clone the repository and run these commands:
```
npm install
npm run generate-key
npm run build
```

It should say:
```
Done, without errors.
```

The extension in crx format will be inside the build/crx/ directory. You can drag it into [extensions] (chrome://extensions) to install locally.

### License

This work is licensed under a GNU GENERAL PUBLIC LICENSE (v2)

### Shoutouts

This package uses the [html2canvas](https://github.com/niklasvh/html2canvas) library written by Niklas von Hertzen.
It also uses the indexedDb wrapper [db.js](https://github.com/aaronpowell/db.js) written by Aaron Powell.
Thank you also to [BrowserStack](https://www.browserstack.com) for providing free chrome testing tools.
