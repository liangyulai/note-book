## [ImageMagick] Dump every frame to a directory from a gif file

``` convert animation.gif target.png ```

If the various frames have transparent areas and build upon each other, you can use the convert command with the "-coalesce" option to produce a set of files target-0.png, target-1.png etc, each of which merges the sequence of previous images:

```convert -coalesce animation.gif target.png```
