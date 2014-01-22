fne
===

FNE's Not Ext

The Basics
===
FNE has grown out of a distaste for Sencha's handling of Ext after ExtJS. Yes
ExtJS can be used free-of-charge, as long as you don't use it commercially. FNE
intends to be more like Ext-Core, which is missing it's download page on Sencha's
site (and has been for some time now). FNE plans to pick up where Sencha left
off, including extending features and adding more modern browser support to
the mix.

Getting Started
===
This is still in early development, so there isn't much done other than adding
some user agent checking for newer IEs (post-8), Android, and iOS. The starting
goals are to work out some cross-platform tweaks (getting the ENTER key code
in IE7; implementing "click" event on Android's native browser). Also, splitting
the main debug file into smaller chunks and adding a build script to create
a minified version.

Using It
===
Download FNE and then

    <script src="/path/to/fne.js"></script>

Most everything is just like Ext Core at the moment, with `Ext` becoming `F`

    F.get('some-el');
    F.Ajax.request({...});

Features
===
One of the goals of FNE is to modernize a library that was left unchanged since version 3.1.0, while the commerical
and robust version is now getting into the later years of it's 4.x release. Some of the features currently available
include more `.is\*` methods:

	// IE updates
	isIE9
	isIE9Compat
	isIE10
	isIE10Compat
	isIE11

	// Mobile updates
	isAndroid
	isAndroidPhone
	isiOS
	isiPad
	isiPhone

Planned features include session handling, history support, and localStorage; to name a few.

Changelog
===
Version 0.1
 * Officially give it a version #

Version 0
 * Add F\_COMAPT flag for Ext backward-compatability

Before Version 0
 * Added a number of `F.is\*` helpers

Why Another Framework???
---
I absolutely love working with Ext Core for doing my general JS work, but it's
been abandoned as Sencha has moved on to bigger things - I can't blame them,
the work on ExtJS and their other services is quite demanding and a much better
investment of their time in terms of time = money. I've used jQuery extensively,
and I don't much care for it...my two cents. I haven't tried many other frameworks,
but I'm sure they're swell. 
