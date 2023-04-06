# Conventional Commits for JavaScript Projects

## 📝 Description

This is a template for configuring conventional commits in JavaScript projects. With consistently structured commit messages, you can automate the generation of changelogs, versions, and release notes, making it easier to track project progress and version management.

## 🚀 Installation

Add the following to the "devDependencies" section of the "package.json" file:

```json
  "devDependencies": {
    "@commitlint/cli": "^17.4.2",
    "@commitlint/config-conventional": "^17.4.2",
    "husky": "^8.0.3",
    "lint-staged": "^13.0.3",
    "prettier": "^2.7.1",
    "standard-version": "^9.5.0"
  }
```

Add the following scripts:

```json
  "scripts": {
    "pre-commit": "lint-staged",
    "postinstall": "husky install",
    "release": "standard-version",
    "test": "echo 'lorem ipsum'"
  },
```

And lastly, add the following configuration:

```json
  "prettier": {
    "semi": true,
    "tabWidth": 2,
    "singleQuote": true,
    "printWidth": 100,
    "trailingComma": "all"
  },
  "commitlint": {
    "extends": [
      "@commitlint/config-conventional"
    ]
  },
```

Once you've added these configurations, run:

```
yarn
```

## 🛠️ Usage

Copy the .github and .husky folders into your project, along with the .versionrc file.

## 💻 Contributing

Thank you for considering contributing to this project! If you'd like to make a contribution, follow these steps:

Fork the repository.
Clone the forked repository to your computer.
Create a new branch and make your changes on that branch.
Push the changes to your forked repository.
Open a pull request in this repository.
Be sure to follow the contribution guidelines before opening a pull request.

## 📜 Credits

This template was created by [Mex Delgado](https://github.com/rudemex)
 and [Fede Loterstein](https://github.com/fedeloterstein)

