# Debugging Angular-CLI Apps in VSCode via Browser Preview

[Check out the full write-up on Medium here!](https://medium.com/@MarkPieszak/debugging-angular-cli-inside-vscode-with-browser-preview-8dcc4b18ed64)

Launch.json changes needed to sync up with the Angular-CLI:

```json
{
  "version": "0.2.0",
  "configurations": [
    {
      "type": "browser-preview",
      "name": "Browser Preview: Attach",
      "request": "attach"
    },
    {
      "type": "browser-preview",
      "request": "launch",
      "name": "Browser Preview: Launch",
      "url": "http://localhost:4200", // <-- 
      "webRoot": "${workspaceFolder}" // <-- 
    }
  ]
}

```


----

## DevHelp.Online - Consulting | Training | Development

Check out **[www.DevHelp.Online](http://DevHelp.Online)** for more info! Twitter [@DevHelpOnline](http://www.twitter.com/DevHelpOnline)

Contact us at <hello@devhelp.online>, and let's talk about your projects needs.

<p align="center">
    <img src="https://s3.amazonaws.com/media-p.slid.es/uploads/768119/images/4272479/Screen_Shot_2017-10-27_at_6.58.34_PM.png" alt="DevHelp.Online - Angular ASPNET JavaScript Consulting Development and Training">
</p>

[![Twitter Follow](https://img.shields.io/twitter/follow/MarkPieszak.svg?style=social)](https://twitter.com/MarkPieszak)
