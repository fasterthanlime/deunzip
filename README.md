## Intro

Ever dealt with .zip files that extract not in their own folder and pollute a whole directory structure?

Well, me too. Now it's as easy as 'Home key + type 'de' + type Enter' to fix the disaster! 

## Usage

Let's suppose you've done

    unzip somefile.zip

But somefile has spewn all over your directory with nasty files, just run

    deunzip somefile.zip

To clean up the mess.

Only the files belonging to the .zip archives will be deleted, along with the folders
that the .zip extraction has created. If you already had non-empty folders with the
same name, they won't be deleted.

## Requirements

  * bash (can be downgraded to sh by rewriting [[ ]] tests)
  * mktemp, rm, rmdir, echo, cat, tac, sort, uniq

## Installation

First, read the source - you should be careful what you install on your system.

Then put it somewhere in your PATH, chmod +x and take it away!

## License

Distributed under the terms of the WTFPL Version 2, see http://sam.zoy.org/wtfpl/
