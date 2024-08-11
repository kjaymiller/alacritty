# alacritty

Configuration instructions for setting up alacritty

## File Structure

Where are the main editable files? Is there a dist/build folder that should be ignored?

## Git Update

Ensure this repo is up to date. Pull from GitHub

@run(git pull)

## Build

What build system/parameters does this use?

@include(Git Update)

```run install alacritty
result=$(brew list alacritty)
if [ -z "$result" ]; then
  brew install alacritty;
else
  brew upgrade alacritty
fi
```

Next install the catppuccin-alacritty theme

```run download catppucin-alacritty
ls ../catppuccin-alacritty
if [ $? -ne 0 ]; then
  gh repo clone catppuccin/alacritty ../catppucin-alacritty
fi
```

## Deploy

What are the procedures/commands to deploy this project?

## Other

Version control notes, additional gulp/rake/make/etc tasks...

```

```
