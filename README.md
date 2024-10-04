# Setup React Native on MAC

- Install homebrew

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

- Run these commands in your terminal to add Homebrew to your PATH:

```bash
echo >> /Users/subratakumardas/.zprofile
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/subratakumardas/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

- install node and watchman

```bash
brew install node
brew install watchman
```

## IOS Setup

- Install XCode

follow [this](https://reactnative.dev/docs/set-up-your-environment?platform=ios#xcode) link to install XCode.

## Android Setup 

- Java Development Kit

```bash
brew install --cask zulu@17

# Get path to where cask was installed to double-click installer
brew info --cask zulu@17
```

After the JDK installation, add or update your JAVA_HOME environment variable in ~/.zshrc (or in ~/.bash_profile) .

If you used above steps, JDK will likely be located at /Library/Java/JavaVirtualMachines/zulu-17.jdk/Contents/Home:

```bash
export JAVA_HOME=/Library/Java/JavaVirtualMachines/zulu-17.jdk/Contents/Home
```

The Zulu OpenJDK distribution offers JDKs for both Intel and M1 Macs. This will make sure your builds are faster on M1 Macs compared to using an Intel-based JDK.

- Install android studio

[link](https://developer.android.com/studio/index.html) to download android studio

after this follow the [official documentation](https://developer.android.com/studio/index.html)


