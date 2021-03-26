# Formation Git Elephorm

Throughout this lab, we will try to write a converter

We want our application to know how to do several things:

### Writing titles

# h1
## h2
### h3
#### h4
##### h5
###### h6

### Make elements bold

**like here**

### Put crossed out elements
(does not work under github)

~~ like here ~~

### Italicize items

*as the*

### Write links

Here is the reference documentation for [markdown] (http://en.wikipedia.org/wiki/Markdown) and [HTML] (http://en.wikipedia.org/wiki/HTML).

### Write numbered lists or not

1. However, they also denounce the error sit involvement
2. The one who, corrupted by the flattery of the present and the pleasures deleniti
  * And the pain and hardship that they are welcome
  * * Blinded by the desire to provide ** no ** *
  And this is the difference between simple and easy
    1. For any further
    2. The pain itself
    3. For carrots
    4. wants to obtain enhanced
3. Who has any right to criticize
4. who is a pleasure that

### Show dividing lines

---

### Write code


```
    var md   = document.getElementById("md").value,
    html = micromarkdown.parse(md);

```

### To be able to reference links on social networks.
(does not work under github)

* Twitter @elephorm@t
* GitHub @sabativi@gh
* Facebook @elephorm@fb
* Google+ @elephorm@gp

## How the application works

### Dependencies

The application is developed in [nodejs] (https://nodejs.org). For more information click on the link.

It needs the [node package manager] (https://www.npmjs.com) to install the dependencies.

You must have `nodejs` and` npm` installed on your machine. The nodejs installer is present [here] (https://nodejs.org/download/). Npm is installed with node. If you want more information including a presentation video, it's [here] (https://docs.npmjs.com/getting-started/installing-node).

Also make sure you have a github account.

Once done, you must:

1. Fork the repository: by clicking on the fork button at the top right. This will be your copy of the server where you can share changes.
2. Go into the directory: `cd Realtime-Markdown-Viewer`
3. Install dependencies: `npm install`
4. Start the application: `npm run dev`
5. Go to this [url] (http: // localhost: 8000)

You should end up with this as a screen:! [] (./ docs / result.png)

### Operation for the TP.

The directory that interests us is the `converter` directory. You will not need to manipulate other files.

The latter has the following structure:

* **markdown.js**
* tests/
	* markdown-test.js
	* **features/** 
	* utils.js

The `markdown` file contains the parser.

The `features` directory contains a set of markdown and html files for our tests.

When we add a new feature, we will accompany it with a test, in order to verify its correct functioning.

To add a test, just add a markdown file and an html file with the same name in the directory.

To run the tests, the command to run at the root of the project is:

```
npm run test
```


On the left you have the panel where you can write markdown and on the right HTML rendering.


We have already developed a feature for you. The parsing of the different titles.

Try the following code in the left panel:

```
# A great title
### A smaller title
##### Must match a <h5> tag
 
```

You should have the right panel which updates automatically.

On the other hand, if you try to write:

```
** This text must appear in bold **
```

You can see that nothing is happening.

Throughout this lab, we will be adding features to our Markdown parser.

The goal of the lab is not to make the parser, we use it as a pretext to use git, all the answers will be given to you during the lab, on the other hand, you need to understand what you are doing when using commands git.




