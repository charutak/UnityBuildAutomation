# Auto Unity build and publish To Itch.io

#### A simple tool for building a Unity project and uploading it to an (existing)itch project page, when new changes are pushed to main(master).
#### It uses [Unity Builder](https://github.com/marketplace/actions/unity-builder) with [Butler Push](https://github.com/marketplace/actions/butler-push) to get the job done.


### Install Instructions:

1. Copy the script [buildAllPlatforms.yml](buildAllPlatforms.yml) to .github/workflows/
2. Add all the platforms to build for the project under target platforms. For a whole list of target platforms and platform specific settings checkout  https://game.ci/docs/introduction/getting-started.
3. Setup the secrets of Unity licence using instructions from [here](https://game.ci/docs/github/activation). 
4. Setup the secret for butler using [this](https://itch.io/docs/butler/login.html#running-butler-from-ci-builds-travis-ci-gitlab-ci-etc). 
5. Create the page in itch.io and setup the project name and username field. 

This is a preliminary setup for the build pipeline, feel free to update it as per personal use case all the details are in the two github action runners.
