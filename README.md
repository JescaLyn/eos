## EOS-Redux

### Background

Redux is a highly efficient application of Flux, a frontend technology used for updating frontend state and re-rendering appropriately. However, Redux, despite requiring fairly consistent files and file structure, has no framework for easily implementing a Redux application. EOS-Redux aims to solve this issue. With Paul Oliva and Alex Mattson, I will be building out EOS-Redux to be a fully functional framework for any Redux application.

### Functionality & MVP

In addition to quickly generating Redux files from the command line, users will be able to:

- [ ] Add any reducer/middleware and see it automatically added to the root reducer/master middleware.
- [ ] Allow EOS to manage the store, including using normalizr to create a standard store shape.
- [ ] Use imported actions and packages without expressly stating so.
- [ ] Integrate with one of many backend options, including Firebase, Rails, and Node Express.

### Wireframes

EOS will help generate files and file structure out of the command line.

### Technologies & Technical Challenges

This package will be constructed using JavaScript as well as packages such as `chalk`, `commander`, and `to-snake-case`.

There will be a primary `eos-cli.js` script as well as many other scripts, including `actions.js`, `util.js`, and template scripts to help construct files.

The primary technical challenges will be:

- Abstracting imports such that users never need to import files and the right files are required in the right places
- Determining how store state will look and implement normalizr
- Integrating various backend possibilities with EOS for seamless applciation to any Redux application

### Implementation Timeline

**Day 1**: Implement adding to root reducer/master middleware when any reducer/middleware is generated. Goals for the day:

- Functioning `sed` command that edits appropriate files.
- Appropriate placement of reducers/middleware.

**Day 2**: Research abstracting imports. Goals for the day:

- Determine how to make a "blind" import.
- Determine the appropriate file tree structure for imports.

**Day 3**: Implement abstracting imports. Goals for the day:

- Provide appropriate functions/packages to Redux cycle components without explicit stating of imports.
- Offer "test" options which imports functions directly to `index.jsx`.

**Day 4**: Refine any other details the package needs. Goals for the day:

- Ensure EOS has a polished user interface as well as careful documentation.
- Assist collaborators in finalizing any goals for EOS.
