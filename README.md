# RulePad

Good documentation offers the promise of enabling developers to easily understand design decisions. 
Unfortunately, in practice, design documents are often rarely updated, becoming inaccurate, incomplete, and untrustworthy. 
A better solution is to enable developers to write down design rules which may be checked against code for consistency. 
But existing rule checkers require learning specialized query languages or program analysis frameworks, offering a barrier to writing project-specific rules. 
We introduce two new authoring techniques for design rules: snippet-based authoring and semi-natural-language authoring.
In snippet-based authoring, developers specify characteristics of elements to match by writing partial code snippets. 
In semi-natural language authoring, a textual representation offers a representation for understanding design rules and resolving ambiguities, which is bidirectionally synchronized.  
We implemented these approaches in RulePad. 
To evaluate RulePad, we conducted a between-subjects user study with 14 participants comparing RulePad with the PMD Designer, a utility for writing rules in a popular rule checker. 
Overall, participants with RulePad were able to successfully author 13 times more query elements in significantly less time and reported being significantly more willing to use RulePad in their everyday work. 


The result of this work is published in "RulePad: Interactive Authoring of Checkable Design Rules", FSE 2020.

## Website 

[https://devx.cs.gmu.edu/tools/rulepad](https://devx.cs.gmu.edu/tools/rulepad)

## Code

RulePad is an extension of ActiveDocumentation
There are 2 parts: [IDE connector](https://github.com/devuxd/ActiveDocumentation/releases/tag/RulePad) 
and the [Main component](https://github.com/devuxd/active-doc-client/releases/tag/RulePad).

### Working with ActiveDocumentation

- Install _srcML_ version 0.9.5 as instructed [here](https://github.com/devuxd/active-doc-client/wiki#installing-srcml)
- Install the plugin ([`ActiveDocumentationPlugin.zip`](https://github.com/devuxd/RulePad/blob/master/ActiveDocumentationPlugin.zip)) on IntelliJ IDE. The plugin has been tested on IntelliJ 2021.1.
- Unzip [`active-doc-client-RulePad.zip`](https://github.com/devuxd/RulePad/blob/master/active-doc-client-RulePad.zip) and open `index.html`.
- Open a Java project in IntelliJ and place two empty files as described [here](https://github.com/devuxd/active-doc-client/blob/RulePad-version/README.md).

### Expanding ActiveDocumentation (IDE Connector)

- Unzip [`ActiveDocumentationPlugin-RulePad-Source.zip`](https://github.com/devuxd/RulePad/blob/master/ActiveDocumentationPlugin-RulePad-Source.zip) and edit using IntelliJ IDE.

### Expanding ActiveDocumentation (Main Component)
- Install the Main component by unzipping [`active-doc-client-RulePad-Source.zip`](https://github.com/devuxd/RulePad/blob/master/active-doc-client-RulePad-Source.zip) and run `npm install`.
- Run the web app with `npm run start-Mac` (for Mac OS system) or `npm run start-Windows` (for Windows system). The latter command should also work for Linux OS but it is not tested.