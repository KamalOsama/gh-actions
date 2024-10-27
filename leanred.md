- .yml works with idententaion, Indentation matters

- workflows folder must be stored in the .github folder, So git can detect it

- The runner machine doesn't have your code, You need to upload you code on it first (using actions: uses), then set it up (install dependencies, etc...)

- Each runner has a list of an already installed dependencies, You can look in the github docs for each runner installed dependencies, For the upuntu/latest, NodeJS is already installed

- npm ci === npm install
  - The difference is that ci install dependencies in the package-lock.json, install install what's in package.json