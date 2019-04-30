# Snoopdroid

# Debian

In order to run Snoopdroid on Debian you will need to install the following dependencies:

    apt install python3 python3-pip python3-dev build-essential libssl-dev libffi-dev swig android-sdk-platform-tools

Make sure to generate your Android keys with:

    adb keygen ~/.android/adbkey

You can then install Snoopdroid with pip3:

    pip3 install snoopdroid

## Mac

Running Snoopdroid on Mac requires Xcode and [homebrew](https://brew.sh) to be installed.

In order to install adb and other dependencies use:

    brew install homebrew/cask/android-platform-tools
    brew install openssl
    brew install swig

Make sure to generate your Android private key with:

    mkdir $HOME/.android
    adb keygen $HOME/.android/adbkey
    adb pubkey $HOME/.android/adbkey > $HOME/.android/adbkey.pub

You can now install Snoopdroid with pip3:

    pip3 install snoopdroid
