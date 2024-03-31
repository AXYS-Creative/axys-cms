# CMS Tool with Netlify Identity and Eleventy (11ty)

This guide outlines the steps to create a CMS tool leveraging Netlify Identity for authentication and Eleventy (11ty) as the static site generator.

## Prerequisites

- Node.js must be installed on your machine.

## Setup

### 1. Initialize a Node.js Project

- Open your terminal to run the following:
- Run `npm init -y` to create a `package.json` file with defaults.
- Install Eleventy: `npm install @11ty/eleventy --save-dev`.

### 2. Update `package.json`

Modify the `scripts` section in `package.json`:

- Swap the `test` script with below:
- Add `"start": "eleventy --serve"` to run a local development server.
- Add `"build": "eleventy"` for building your site.

### 3. Configure Eleventy

In the root of the project create a `.eleventy.js` with the following content:

```javascript
module.exports = function (eleventyConfig) {
  return {
    dir: {
      input: "src",
      output: "public",
    },
  };
};
```

### 4. npm start

In your terminal run the start command by typing `npm start` as declared in our `package.json`

```javascript
module.exports = function (eleventyConfig) {
  // Eleventy configuration goes here
};
```
