# What is it

Dependency updater is a simple script that add dependencies for custom packages.

This is a feature that won't be added into Unity for security reasons.

To be able to add custom dependencies, you have to add a "customDependencies" array on your **package.json** file like the sample below. This script is part of a exercice I've made to be able to share packages I make for Unity: I explain in this [Medium post](https://medium.com/p/1339880dd09) why I wrote it and why I don't use it, but it's freely available for you to understand the process.

```json
{
  "name": "com.fredericrp.assetbundle",
  "version": "1.0.0",
  "displayName": "FredericRP Asset Bundle Tool",
  "description": "Tool for Asset Bundles - FredericRP standard assets",
  "unity": "2020.1",
  "unityRelease": "0f1",
  "dependencies": {
 },
 "customDependencies": [
	"ssh://git@github.com/FredericRP/Standard-Assets.git?path=/Plugins/Singleton"
	],
 "keywords": [
    "standard assets"
  ],
  "author": {
    "name": "FredericRP",
    "email": "unity@FredericRP.com",
    "url": "https://FredericRP.com"
  }
}
```
