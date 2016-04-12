LockPages Public API + Example Projects
=======================================

LockPages is a support package for other tweaks (like [Forecast](https://cydia.angelxwind.net/dba-tech/?page/com.dba-tech.forecast)) to add pages to the lock screen.

### Setting up your development environment (assuming you already have [Theos](https://github.com/theos/theos))

1. Copy `LPPage-Protocol.h` and `LPPageController.h` to `$THEOS/include/lockpages/`

1. Copy `liblockpages.dylib` to `$THEOS/lib/`

### How do I use LockPages? Are there any example projects I can look at?

I've written two open-source example projects, which are included in this Git repo: `PineappleSpinnerLS` and `LPBarebonesExample`. (They're both in the `examples/` subfolder.)

`PineappleSpinnerLS` is basically a complete tweak I wrote in 30 minutes or so. It adds a fully-functional page to your lock screen where you can tap a button to spin a pineapple, and tap another button to accelerate it (much to its dismay).

`LPBarebonesExample` is a barebones project that contains just enough code to create a LockPages page and nothing else. The view is completely empty. You can use this project to quickly create a tweak by adding code onto `ExampleView`.

Also, make sure you add `com.dba-tech.lockpages` to your control file's `Depends:` field!