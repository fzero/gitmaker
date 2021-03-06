# Gitmaker v0.5

**Gitmaker** is a simple script that creates a Git repository in a remote SSH
server and clones it in the local machine.

This is only possible because:

1. Git is awesome. No, seriously, it is. While you can do really complicated
forks and merges with it, the way it works over the network is incredibly simple
and decentralized.

2. You don’t have to install any daemons or special modules to have your remote
Git repository (you can if you want to, but it’s not mandatory); the only thing
you need is Git itself.

To use Gitmaker you need:

* Git installed on both your local machine and the SSH server. 
* Key-based login configured for your SSH user (optional but highly recommended, unless you like to type your password a lot).

Once you have this, go to your favorite folder where you keep your precious programming projects and type:

```sh
gitmaker your_user@example.com myrepo
```

This will create a remote `myrepo` repository at `example.com` with a local clone
on the current directory. Yep, it’s ready. Commit and be happy.


## OMG bonus round!

Use the [`coolgit`](coolgit) sccript to add some color and aliases to your git setup. It can
also setup your global username, email and ignore file. Just jump in and edit it
to your liking.


## Micro-FAQ

**Q: But dude, I don’t have Git on my server!**

A: Well, that sucks. Anyway, it shouldn’t be too complicated to fix this.

If you have root access, just `apt-get install` it (or `yum` it, or `emerge` it —
whatever you like). If you don’t, I believe it shouldn’t be too complicated
to compile it from source with `PREFIX=/home/your_user`.


**Q: But I run Windows!**

A: This should work fine on WSL (a.k.a. Ubuntu on Windows) or any other *nix-on-
Windows tools such as Cygwin. Yes, you will need to use a terminal, but if
you're here you probably know that already!


## License

Hey, it's on GitHub. Anyone can see, anyone can fork, anyone can modify. Just
to formalize this stuff, Gitmaker is under the Artistic License 2.0 - not only
to piss off Richard Stallman fans, but also because the GPL v3 is ridiculously
restrictive and paranoid. So no soup for you, Stallman. It's probably a good
thing too, since we know soup and beards don't mix very well.

http://www.opensource.org/licenses/artistic-license-2.0.php


## Contact

If you really want, you can follow me on Twitter:
[@fzero](https://twitter.com/fzero). Beware: I write both in English and
Portuguese, post lots of cat pictures and I'm leftwing AF.
