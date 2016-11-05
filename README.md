# Stata - Applied Economics

## About this introduction

This introduction provides a stripped-down overview of some of the features, and commands available within Stata, as well as helpful examples of the features in their context.

Examples within this document are built 

## Using a .do file

Stata supports interactive or .do file command execution. While the interactive console can be convenient for experimentation, it is really bad for creating reproducible work, and easily allows errors to enter into your results unnoticed. 

As such always make sure work is written in a `.do` file.

## Commands

### Environment setup

`cd` Sets the *working directory*, which is the default folder from which all other commands will run. This means that your output (e.g. log files) and input (e.g. data files) will all be read from and written to this location by default.

```
cd [path]
```

* `path` the full path to your desired working directory, surrounded by quotation marks if it contains spaces.

e.g.

```
cd "O:\Documents\Applied Economics\Tutorial 2"
```

___

`use` Loads a dataset from your working directory. 

```
use [datafile] *[, clear]*
```

* `datafile` Filename of dataset within working directory, or relative path to working directory.
* `, clear` (**Optional**) Allows data currently stored in variables to be overwritten

e.g. 
```
use DataUoBSet2.dta, clear
```

### Data management

`display` Basic way of outputting data or the output of a calculation to the console. When presented with a list of data, the display option will output the first item

```
display [operation]
```

* `operation` A stata expression to output

e.g.

```
display 1 + 1
```

`list` 

`generate` `gen` creates new variables

`drop`

`replace`

`describe`

`label`

`rename`

`tables`

`summarize`

`tabulate` `tab`

`tabstat`

## Interactive Env

`browse` 

## Maths

`+` `-` `/` `*` `^` Operators

`log` `ln`

`exp`

`sqrt`

`sum`

`min` `max`

`floor` `ceiling` `round`

`int`

### Graph

`histogram`

`kstat`

`plot`

`scatter`

### Execute

`regress` `reg`

`streg`

### Test

`test`

`ttest`

### Survivor Model

`stset`

`sts`

## Useful features

### Factor Variables

http://www.stata.com/help.cgi?fvvarlist

### Special Variables

`return` `r`

`ereturn` 

### log