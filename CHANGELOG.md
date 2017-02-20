# ChangeLog

## 0.5.18 (15 Feb 2017)
* Verbose logging for nimsuggest
* Fix nim check leaks and nimsuggest instance leaks

## 0.5.17 (11 Feb 2017)
* Nim documentation support improvements for hover and code completion

## 0.5.16 (07 Feb 2017)
* Fixed toggle line comment stopped working in .nim files after 0.5.15 update [#35](https://github.com/pragmagic/vscode-nim/issues/35)
* Readded bracket auto closing (it is intended that the string literals are brackets, VSCode recognises this and doesn't show a box around quotation marks)
* Fixed signature completion of iterators
* Fixed two snippets which pasted invalid code

## 0.5.15 (06 Feb 2017)
* Highlight boolean keywords in default schemes (#34)
* Prevent sorting code completion suggestions
* Incorrect indentation after string literal (#32)
* Improve run selected file (#5)

## 0.5.14 (16 Jan 2017)
* Fixed when terminal not appeared after was closed
* Added option for run unsaved content ("nim.runUnsaved" configuration property)

## 0.5.13 (18 Dec 2016)
* Added "Nim: Run file" command that run selected file with `F6` keyboard shortcut
* Fixed "Provide more details in symbols window" [#27](https://github.com/pragmagic/vscode-nim/issues/27)

## 0.5.12 (04 Nov 2016)

* Added support of bundled nimsuggest with compiler that will be available in upcoming Nim 0.15.3 release

## 0.5.11 (23 Oct 2016)

* Fixed nim check multiline result parsing

## 0.5.9 (21 Sep 2016)

* Fixed nim check often hangs and doesn't get killed [#23](https://github.com/pragmagic/vscode-nim/issues/23)
* Fixed signature suggestion wrong behavior [#21](https://github.com/pragmagic/vscode-nim/issues/21)

## 0.5.7 (1 Aug 2016)
* Minor fixes for the signature provider [PR #22](https://github.com/pragmagic/vscode-nim/pull/22)
* Temporary disabled reindex on file change due leak of nimsuggest

## 0.5.5 (1 Aug 2016)
* Added support for parameter hints [PR #19](https://github.com/pragmagic/vscode-nim/pull/19)

## 0.5.4
* Added snippets [PR #18](https://github.com/pragmagic/vscode-nim/pull/18)
* Added a new nimsuggest
* Updated buildOnSave relative to tasks.json
* Fixed [Multiline comments syntax highlight.](https://github.com/pragmagic/vscode-nim/issues/11)
* Minor improvements and stability fixes 

## 0.5.2
* Added multiple projects support
* Fixed some hangs during indexing 

## 0.5.1
* Fixed #12 - Cannot compile nimsuggest 

## 0.5
* Refactored nimsuggest interaction to use EPC mode, removed nimble requirements
* Added info with qualified name for hovered element
* Improved suggest information

## 0.4.10
* Added test project support
* Improved nim check error parsing for macros and templates

## 0.4.9
* Improved database indexes
* Fixed multiline error in nim check
* Fixed nimsuggest problem with mixed case path in windows

## 0.4.6
* Fixed #9 - nimsuggest "attacks" (one process per nim file in workspace)
* Added type index persistence with NeDB

## 0.4.4
* Fixed #7 - Block comments / inline comments are not supported
* Fixed #8 - Terrible experience with clean install w/o nimsuggest

## 0.4.3
* Added workspace symbol search support 
* Rewrote nimsuggest handling to use TCP mode
* Added `nim.licenseString` for inserting default header in new nim files
* Updated `run project` command to run single file in non project mode 