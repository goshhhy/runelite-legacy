****![](https://runelite.net/img/logo.png)
# runelite-legacy

runelite-legacy is a set of patches for [RuneLite](https://github.com/runelite/runelite) to reduce the minimum required
version of Java. Unmodified RuneLite requires Java 11. with these changes, it can currently be built to target Java 9.
My goal is to reduce the requirement to at least Java 1.7 and preferably Java 1.6, even if this requires disabling some
functionality, while still allowing the Java 11 version to be built and retain all of its features.

the patches are minimal, and do not add any new features. some features may be disabled if they rely on language
features or libraries not available in earlier versions of Java. there should be no change whatsoever in behavior of
the client otherwise.

my intent is for these changes to be suitable for merging into the official runelite client, in order to allow an
officially supported build to exist that can run on older computers and operating systems that do not support newer
versions of Java. yes, this is all so that i can play OSRS on my PowerBook G4, like the good old days.

I try to encapsulate changes of the same issue (e.g. occurrences of language features not present in older Java) into
the same commit, in order to keep things clean and easy to review.

### License

runelite-legacy is licensed under the BSD 2-clause license. See the license header in the respective file to be sure.****
