# WoWHelloWorld
A sandbox repo to play around with GitHub actions and WoW addon releasing.

Links to published addon:
- [WoWInterface](https://wowinterface.com/downloads/info26310-WoWHelloWorld.html)
- [CurseForge](https://www.curseforge.com/wow/addons/wowhelloworld)
- [Wago](https://addons.wago.io/addons/wowhelloworld)

All releaes are handled by the GitHub action [`build-addon`](.github/build-addon.yml) and [`build-addon-beta`](./github/build-addon-beta.yml). Each tagged release triggers `build-addon` to create a release on each provider, and each push to the main branch triggers `build-addon-beta`, which creates a release tagged as a beta release in each provider.