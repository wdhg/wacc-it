# wacc-it

`waccit` is a script which can upload wacc programs to an online reference compiler and print the output.

## Install

This script uses the command `jq`. To install on Mac OS:

```
$ brew install jq
```

To install `waccit` simply clone this repo and run the script:

```
git clone git@github.com:wdhg/wacc-it.git
cd wacc-it
./waccit
````

You can either run the script directly or add it to your `PATH`.

## Example

```
$ ./waccit -x test.wacc
Upload
-------
begin
 println "hello world"
end

Compiler out
------------
-- Compiling...
-- Assembling and Linking...
-- Executing...
===========================================================
hello world
===========================================================
The exit code is 0.
-- Finished
```
