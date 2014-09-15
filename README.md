# Generic Ant build files for Zimbra development

## Introduction

If you're developing a Zimbra server extension or a Zimbra zimlet, you'll always 
go through a few steps to build and deploy the extension or zimlet.

These steps can easily be automated using Ant.

This repository contains two generic build environments for server extensions 
and zimlets, that are very easy to use.

## Prerequisites

* [Apache Ant][ant] version 1.9.4 or later
* [Jsch][jsch] Jsch libraries 0.1.51 or later for the deployment processes 
  (put them somewhere ant can reach them. For example in ~/.ant/lib)

## Installation

Grab all files in the serverextension or zimlet directory and put it in the 
root of your server extension or zimlet development path.

Copy the file build\_dist.properties to build.properties and customize that to 
your liking.

## Usage

The build process is simply started using the command "ant" with a target as 
the only parameter.

To get a list of available targets and a description about what they do, use

    ant -p 

[ant]: http://ant.apache.org/
[jsch]: http://www.jcraft.com/jsch/
