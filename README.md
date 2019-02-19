# docker-android-sdk-fastlane
Docker image for automated Android builds and distribution with fastlane tools. An autoupdating of docker hub image is turned on and we will push new version of gradle later.

## Usage

Simply run the container and mount your project to the `/app` folder, then run `fastlane` commands as you usually do.

```
$ docker run --rm -v \ 
  ${PWD}:/app \ 
  opengamer/android-sdk-gradle-fastlane \
  fastlane beta
```

## Docker hub link

https://hub.docker.com/r/opengamer/android-sdk-gradle-fastlane

## What Is Inside

Built upon the `:latest` branch of the great [`runmymind/docker-android-sdk/`](https://hub.docker.com/r/) image. In addition it installs `ruby`, the latest `fastlane` and `gradle 4.6`.

## Inspired by

https://github.com/blackmirror-media/docker-android-sdk-fastlane but with new version of `gradle` 