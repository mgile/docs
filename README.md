SproutCore Documentation Generator
==================================

A tool to generate documentation for the SproutCore framework and SproutCore projects, using the JSDoc format.

**Authors**: Majd Taby, Peter Wagenet

Usage
-----

    gem install sc-docs

*NOTE: If you are not using the latest version of SproutCore, the
built-in sc-docs command may conflict. This has been fixed in the newest
versions of SC.*

### Basic

    sc-docs preview INPUT_DIRECTORY_PATH

This documents the specified directory and then runs a preview sc-server instance.

### Deploy

    sc-docs generate INPUT_DIRECTORY_PATH -o OUTPUT_DIRECTORY_PATH

The generate command runs sc-build and deploys to the specified directory.

### HTML Templates

    sc-docs generate INPUT_DIRECTORY_PATH -o OUTPUT_DIRECTORY_PATH -t TEMPLATE_PATH


By default sc-docs assumes that you want to generate docs for the SproutCore based Doc Viewer. However, if you pass a template it will generate a standard HTML output.

Dependencies
------------

* **node.js**: We use a special (much faster) version of jsdoc-toolkit that requires node.js.

Templates
---------

### sc_fixture

Generates the docs in JSON format for use within an SC based viewer app.

### docs.sproutcore.com

The template used at docs.sproutcore.com. Designed by Matt Grantham and Ryan Mudryk with additional work by Avrohom Katz.

Credits
------

**jsdoc-toolkit**: Used for the heavy lifting of docs generation

