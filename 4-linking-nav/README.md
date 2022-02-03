# Linking and Navigation

Let's exercise our wits about how to write paths that point to different places and files both *relative* and internal to a project and *absolute* and potentially external to it.

## Learning Goals

- Recognizing what the *root* of your project is;
- Writing link / path notation:
- Understanding how to write a conventional `nav` (navigation) menu for a page, using the `ul`, `li`, and `a` elements.

## Exercise

Before you begin, here's a short lesson on paths and navigation menus that reflect the website's folder-file hierarchy.

### Writing Path Notation - How to link and move within your project's structure

- `./` - Begin in the same location as this file and travel from there
- `/`  - Forward-slash denotes moving forward in a project path
- `..` - Two-dot notation travels back 1 folder in your project folder

Since you are working in a subfolder within the html-exercises, you will need to use the `./` notation at the beginning of many of your relative paths.

When the above notations are combined, you can write the following to move out of a folder and into another folder that is above it in the folder tree strtucture:

```
./              Start in this folder, regardless of where this file is located
../             Move up of 1 folder in the folder's tree structure
../../          Move up of 2 folders in the folder's tree structure
../../../       Move up of 3 folders in the folder's tree structure
etc.
```

### Applying paths to a `nav` menu with nested `ul` and `li` elements

You can nest lists, which can help you create a navigation menu that reflects your folder-file structure. For example, take the following website structure:

```
*lindgren
  |_ index.html
  |
  |_ /publications
  |   |_ index.html
  |   |_ articles.html
  |   |_ chapters.html
```

The `nav` menu in the parent folder's `index.html` nests `ul` elements in the code below to reflect this folder-file hierarchy. 

- **Note**: This can be accomplished in a couple ways, so this is one possible structure.
- **Reflect** on my use of the relative URL path notation to tell computers where to find a file.

See and test this code in action in the provide `lindgren` example.

```
<nav>
  <ul>
    <li>
      <a href="index.html">Home</a>
    </li>
    <li>
      <a href="./publications/index.html">Publications</a>
      <ul>
        <li>
          <a href="./publications/articles.html">Articles</a>
        </li>
        <li>
          <a href="./publications/chapters.html">Chapters</a>
        </li>
      </ul>
    </li>
  </ul>
</nav>
```

## Writing Your Navigation Menu

### 1. Create the following project folder structure within this exercise folder

Setup your project parent folder by **using your lastname** like my example below:

```
*lindgren
  |_ index.html
  |
  |_ /about
  |   |_ index.html
  |   |
  |   |_ /team
  |      |_ team1.html
  |      |_ team2.html
  |
  |_ /contact
     |_ index.html
```

### 2. Write out the *breadcrumb* in every .html file

Inside of every .html file, write the breadcrumb within an h1 element. See my example for reference.

**Don't skip this!** This is important, because it will help you and me test your navigation by providing the file's location relative to the project's parent folder.

### 3. Create a `nav` in your parent folder's `index.html`

1. Inside this `index.html` page, write a simple HTML document with the baseline elements: `doctype`, `html`, `head` with some basic info, and `body`.
2. Inside the `body`, write a `nav` menu with an `ul` that provides relative links (`a`) to all of the pages.
3. Test your navigation links before moving onto the next step.

### 4. Create a `nav` in `team1.html`

1. Inside the `team1.html` page of the site, write a simple HTML document with the usual basic elements. 
2. Inside the `body` of `team1.html`, write a `nav` menu with an `ul` that provides relative links (`a`) to all of the pages.
3. Test your navigation links before moving onto the next step.

### 5. Create your own nested folder and files within your parent folder

1. Inside your parent folder, create and name another subfolder of your own choosing. 
2. Create an `index.html` file in it, as well as one more subfolder with 1 `.html` page of your choosing.
3. Like the previous steps, create a basic page structure and navigation menu.
4. Update all of you navgivation menus with the appropriate links.
5. Test your navigation links before moving onto the next step.

### 6. Add an absolute link on the home page

1. Return to your home page: the `index.html` file in your parent folder.
2. After the `nav` element, add a simple paragraph (`p`) with linked text (`a`) that uses an *absolute URL* to our ENGL-4814 organization on Github.com: https://github.com/engl-4814

### 7. Again, test the navigation links on your pages before submitting

1. Test your code on your local computer before committing and pushing it to Github.
2. Test your code at the live, online version via the URL.
3. Submit it, if every link works.
