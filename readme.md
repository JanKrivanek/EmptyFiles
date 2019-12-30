<!--
GENERATED FILE - DO NOT EDIT
This file was generated by [MarkdownSnippets](https://github.com/SimonCropp/MarkdownSnippets).
Source File: /readme.source.md
To change this file edit the source file and then run MarkdownSnippets.
-->

# <img src="/src/icon.png" height="30px"> EmptyFiles

[![Build status](https://ci.appveyor.com/api/projects/status/4mrhpal9rwtqajws/branch/master?svg=true)](https://ci.appveyor.com/project/SimonCropp/EmptyFiles)
[![NuGet Status](https://img.shields.io/nuget/v/EmptyFiles.svg?label=EmptyFiles)](https://www.nuget.org/packages/EmptyFiles/)

A collection of minimal binary files.

<!-- toc -->
## Contents

  * [NuGet package](#nuget-package)
  * [Files](#files)
  * [Usage](#usage)
    * [GetPathFor](#getpathfor)
    * [IsEmptyFile](#isemptyfile)
    * [AllPaths](#allpaths)<!-- endtoc -->

## NuGet package

 * https://nuget.org/packages/EmptyFiles/


## Files

All files: https://github.com/SimonCropp/EmptyFiles/tree/master/files

<!--
include: extensions
path: /src/EmptyFiles.Tests/extensions.include.md
-->
  * 7z (32 bytes)
  * bmp (58 bytes)
  * bz2 (14 bytes)
  * dds (136 bytes)
  * dib (58 bytes)
  * docx (1.9 KB)
  * emf (620 bytes)
  * exif (734 bytes)
  * gif (799 bytes)
  * gz (29 bytes)
  * ico (70 bytes)
  * j2c (270 bytes)
  * jfif (734 bytes)
  * jp2 (355 bytes)
  * jpc (270 bytes)
  * jpe (734 bytes)
  * jpg (734 bytes)
  * jxr (300 bytes)
  * odt (2.2 KB)
  * pbm (8 bytes)
  * pcx (131 bytes)
  * pdf (280 bytes)
  * pgm (12 bytes)
  * png (119 bytes)
  * ppm (14 bytes)
  * pptx (13.3 KB)
  * rle (58 bytes)
  * rtf (6 bytes)
  * tar (1.5 KB)
  * tga (543 bytes)
  * tif (250 bytes)
  * wdp (300 bytes)
  * webp (228 bytes)
  * wmp (300 bytes)
  * xlsx (4.5 KB)
  * zip (22 bytes)


## Usage


### GetPathFor

Gets the path to an empty file for a given extension

<!-- snippet: GetPathFor -->
<a id='snippet-getpathfor'/></a>
```cs
var path = EmptyFiles.GetPathFor("jpg");
```
<sup><a href='/src/EmptyFiles.Tests/Tests.cs#L13-L15' title='File snippet `getpathfor` was extracted from'>snippet source</a> | <a href='#snippet-getpathfor' title='Navigate to start of snippet `getpathfor`'>anchor</a></sup>
<!-- endsnippet -->


### IsEmptyFile

Returns true if the target file is an empty file.

<!-- snippet: IsEmptyFile -->
<a id='snippet-isemptyfile'/></a>
```cs
var path = EmptyFiles.GetPathFor("jpg");
Assert.True(EmptyFiles.IsEmptyFile(path));
var temp = Path.GetTempFileName();
Assert.False(EmptyFiles.IsEmptyFile(temp));
```
<sup><a href='/src/EmptyFiles.Tests/Tests.cs#L23-L28' title='File snippet `isemptyfile` was extracted from'>snippet source</a> | <a href='#snippet-isemptyfile' title='Navigate to start of snippet `isemptyfile`'>anchor</a></sup>
<!-- endsnippet -->



### AllPaths

Enumerates all empty files

<!-- snippet: AllPaths -->
<a id='snippet-allpaths'/></a>
```cs
foreach (var path in EmptyFiles.AllPaths)
{
    Trace.WriteLine(path);
}
```
<sup><a href='/src/EmptyFiles.Tests/Tests.cs#L36-L41' title='File snippet `allpaths` was extracted from'>snippet source</a> | <a href='#snippet-allpaths' title='Navigate to start of snippet `allpaths`'>anchor</a></sup>
<!-- endsnippet -->


## Release Notes

See [closed milestones](../../milestones?state=closed).


## Icon

[Hollow](https://thenounproject.com/term/hollow/51835/) designed by [Michael Senkow](https://thenounproject.com/mhsenkow/) from [The Noun Project](https://thenounproject.com).
