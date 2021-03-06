<img src="https://raw.githubusercontent.com/1egoman/biome/master/resources/logo.png" style="width: 300px;" />

# Biome
A shell script to manage your app's environment.
<!--
Biome stores the makeup of your app's environment, so when a new user or contributor wants to run
your app, Biome prompts them for all required secrets. 

Biome saves all your secrets in one place, away from version control. Environment details never
leave your local system.
-->
## Install
Biome is written in bash, and can be installed by running:
```bash
curl https://raw.githubusercontent.com/1egoman/biome/master/biome.sh > /usr/local/bin/biome && sudo chmod +x /usr/local/bin/biome
```
For help, run `biome help`.

## Usage
![Biome: Getting Started](https://raw.githubusercontent.com/1egoman/biome/master/resources/Getting Started.png)

## FAQ
- **How do I change an environment later on?** `biome edit [project name]`.

- **What's the difference between `biome use` and `biome use [project name]`?**
Omitting a project name tells Biome to look in the current directory for a Biomefile. If found,
the specified name will be used in place of the passed project name.

- **Is there an easy way to tell which environment I'm in within a shell created by biome use?**
Biome sets a few additional environment variables (see all with `env | grep BIOME`), one of
them being `BIOME_PROJECT`. This contains the name of the current project that has been loaded from
the environment.

- **Do I have to install Biome globally?**
No. Some choose to install Biome locally (in the root of the project), which makes the process of
contributing easier for others.

- **I'm having problems. Help me!**
If you can't figure out a problem on your own, leave an issue and I'll take a look.

- **I want to contribute.**
Great! Pull requests are always welcome.

----------
Created by [Ryan Gaus](http://rgaus.net)
