# Moreutils

This is a tap that provides a `moreutils` Formula for [Homebrew](https://brew.sh/) with additional options.

BEGIN @arbal FORK NOTES

This fork just adds a one-liner to do all the updates and cleanup and will likely help me out again in the future. I hope it helps *you* too.

`echo "Thank you @slhck for https://github.com/slhck/homebrew-moreutils :)"`

`brew update; brew uninstall -f --ignore-dependencies parallel; brew uninstall -f --ignore-dependencies task-spooler; brew uninstall -f --ignore-dependencies moreutils; brew update; brew upgrade; brew cleanup; brew tap-pin slhck/moreutils; brew update; brew upgrade; brew install moreutils --without-parallel --without-errno --without-ts; brew install -f parallel; brew install -f pwntools; brew install -f task-spooler; brew update; brew upgrade; brew cleanup; brew doctor`

(https://gist.github.com/arbal/3f552be79d279f30f461d401a5716641)

OR

`source <(curl -s https://gist.githubusercontent.com/arbal/3f552be79d279f30f461d401a5716641/raw)`

END @arbal FORK NOTES

## Options

The formula supports the following options:

- `--without-parallel`: Build without the 'parallel' tool
- `--without-errno`: Build without the 'errno' tool, for compatibility with 'pwntools'
- `--without-ts`: Build without the 'ts' tool, for compatibility with 'task-spooler'

## How do I install these formulae?

`brew install slhck/moreutils/moreutils`

Or `brew tap-pin slhck/moreutils` and then `brew install moreutils`.

Or install via URL (which will not receive updates):

```
brew install https://raw.githubusercontent.com/slhck/homebrew-moreutils/master/Formula/moreutils.rb
```

## Documentation

`brew help`, `man brew` or check [Homebrew's documentation](https://docs.brew.sh).
