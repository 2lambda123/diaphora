# Diaphora

Diaphora (διαφορά, Greek for 'difference') version 3.0 is the most advanced program diffing tool (working as an IDA plugin) available as of today (2023). It was released first during SyScan 2015 and has been actively maintained since this year: it has been ported to every single minor version of IDA since 6.8 to 8.3.

Diaphora supports versions of IDA >= 7.4 because the code only runs in Python 3.X (Python 3.11 was the last version being tested).

## Unique Features

Diaphora has many of the most common program diffing (bindiffing) features you might expect, like:

 * Diffing assembler.
 * Diffing control flow graphs.
 * Porting symbol names and comments.
 * Addig manual matches.
 * Similarity ratio calculation.
 * Batch automation.
 * Call graph matching calculation.
 * Dozens of heuristics based on graph theory, assembler, bytes, functions' features, etc...

However, Diaphora has also many features that are unique, not available in any other public tool. The following is a non extensive list of unique features:

 * Support for compilation units (finding and diffing compilation units).
 * Microcode support.
 * Parallel diffing.
 * Pseudo-code based heuristics.
 * Pseudo-code patches generation.
 * Ability to port structs, enums and typedefs.
 * Diffing pseudo-codes (with syntax highlighting!).
 * Scripting support (for both the exporting and diffing processes).
 * ...

## Donations

You can help (or thank) the author of Diaphora by making a donation, if you feel like doing so: [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&amp;hosted_button_id=68Z4H8SE7N64L)

## License

Versions of Diaphora prior to 1.2.4, including version 1.2.4, are licensed under the [GNU GPL version 3](https://www.gnu.org/licenses/gpl-3.0.html). Since version 2.0, Diaphora is now licensed under the [GNU Affero GPL version 3 license](https://www.gnu.org/licenses/agpl-3.0.html). The license has been changed so companies wanting to modify and adapt Diaphora cannot offer web services based on these modified versions without contributing back the changes.

For 99.99% of users, the license change doesn't affect them at all. If your company needs a different licensing model, check the next section...

## Licensing

Commercial licenses of Diaphora are available. Please contact admin@joxeankoret.com for more details.

## Documentation

You can check the tutorial https://github.com/joxeankoret/diaphora/blob/master/doc/diaphora_help.pdf

## Screenshots

This is a screenshot of Diaphora diffing the PEGASUS iOS kernel Vulnerability fixed in iOS 9.3.5:

![Diffing iOS 9.3.5 diff](http://sektioneins.de/images/diaphora1.png)

And this is an old screenshot of Diaphora diffing the [Microsoft bulletin MS15-034](https://technet.microsoft.com/en-us/library/security/ms15-034.aspx):

![Diaphora diffing MS15-034](https://pbs.twimg.com/media/CCnruP_W0AA8ksc.png:large)

These are some screenshots of Diaphora diffing the [Microsoft bulletin MS15-050]( https://technet.microsoft.com/en-us/library/security/ms15-050.aspx), extracted from the blog post [Analyzing MS15-050 With Diaphora](http://www.alex-ionescu.com/?p=271) from Alex Ionescu.

![Diaphora diffing MS15-050, best matches](http://www.alex-ionescu.com/wp-content/uploads/diaphora2.png)
![Diaphora diffing MS15-050, partial matches](http://www.alex-ionescu.com/wp-content/uploads/diaphora3.png)
![Diaphora diffing MS15-050, diffing pseudo-code](http://www.alex-ionescu.com/wp-content/uploads/diaphora1.png)

![Diaphora diffing a LuaBot, matches and pseudo-code](https://1.bp.blogspot.com/-O5UjSOyjCgg/V5byA-ozXVI/AAAAAAAABaY/yRTMDTSD9zI0mSy4AsHN21ZYf_YvctnkwCLcB/s1600/evs-compile.png)


Here is a screenshot of Diaphora diffing [iBoot from iOS 10.3.3 against iOS 11.0](https://blog.matteyeux.com/hacking/2018/04/04/diaphora-diff-and-ida.html):

![Diaphora diffing iBoot from iOS 10.3.3 against iOS 11.0](https://blog.matteyeux.com/images/newgraph.PNG)
