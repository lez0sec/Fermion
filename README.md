# Fermion

Fermion is an electron application that wraps [frida-node](https://github.com/frida/frida-node) and [monaco-editor](https://microsoft.github.io/monaco-editor/). It offers a fully integrated environment to prototype, test and refine Frida scripts through a single UI. With the integration of Monaco come all the features you would expect from Visual Studio Code: Linting, IntelliSense, keybindings, etc. In addition, Fermion has a TypeScript language definition for the Frida API so it is easy to write Frida scripts.

What's in a name: A fermion can be an elementary particle, such as the electron, or it can be a composite particle, such as the proton. Fermions include all quarks and leptons, as well as all composite particles made of an odd number of these, such as all baryons and many atoms and nuclei.

## How to get Fermion?

### Run Fermion from source

Download the repository and navigate to the "Fermion" folder in the terminal. Once there, set the following environment variables.

```
# Windows
set npm_config_runtime=electron
set npm_config_target=5.0.0

# Linux / OSX
export npm_config_runtime=electron
export npm_config_target=5.0.0
```

Afterwards install the packages required to run Fermion with:

```
npm install
```

Once complete, you can run Fermion by issuing:

```
npm start
```

### Compile a release package

Complete the steps above and then issue the following command from the terminal:

```
# Windows
electron-packager . --icon assets\img\fermion-ico.ico

# Linux
electron-packager . --icon assets/img/fermion-ico.png

# OSX
electron-packager . --icon assets/img/fermion-ico.icns
```

### Releases

You can get the latest pre-built Fermion for x64 Windows from [releases](https://github.com/FuzzySecurity/Fermion/releases).

## Eye candy

You can see a sample of Fermion at work below.

![Fermion](Images/Fermion-1.png)

Fermion has auto-complete, linting and Frida API symbol definitions.

![Help](Images/Fermion-2.png)

## Notes

### ChangeLog

For more details on version specific changes consult the [changelog](https://github.com/FuzzySecurity/Fermion/blob/master/CHANGELOG.txt).

### Call to action

If you integrate Fermion into your work-flow and find it useful I encourage you to make pull requests, submit bug reports and ask for features to improve the application. I'm not exactly a Node developer so I am sure people will find ways optimize and rework some of the components.

### Special thanks

I just want to give a few special thanks!

* A huge thanks to [Ole André V. Ravnås](https://twitter.com/oleavr) for all his work on Frida and having a lot of patience answering my pedestrian questions about Frida, NodeJS and Monaco!
* A shout-out also to [mattahan](https://www.deviantart.com/mattahan). I'm using a Buuf icon for the Windows package of Fermion. I'm sure we have all used some of his icons on NIX over the years.