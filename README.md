# Mercurial4Chorus

This repo contains the binaries (Windows as well as Linux 32- and 64-bit) and extensions for the
Mercurial version that Chorus uses. Mercurial is provided in the form of a nuget package,
[SIL.Chorus.Mercurial](https://www.nuget.org/packages/SIL.Chorus.Mercurial).

After installation of the nuget package the `Mercurial` and `MercurialExtensions` folders will be
copied to the solutions directory during the build.

## Building

To create a pre-release nuget package:

```bash
msbuild /p:BuildCounter=1 build/SIL.Chorus.Mercurial.proj
```

To release a nuget package:

```bash
msbuild /p:PreRelease=. build/SIL.Chorus.Mercurial.proj
```
