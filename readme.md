# TypeScript Project Setup

This README explains how to initialize, configure, build, and run a basic **TypeScript** project using Node.js.

---

## Prerequisites

Make sure you have the following installed:

* **Node.js** (v16 or above recommended)
* **npm** (comes with Node.js)

Check versions:

```bash
node -v
npm -v
```

---

## Step 1: Initialize the Project

Create a new project folder and initialize npm:

```bash
npm init -y
```

This will generate a default `package.json` file.

---

## Step 2: Install TypeScript

Install TypeScript as a development dependency:

```bash
npm install --save-dev typescript
```

Verify installation:

```bash
npx tsc --version
```

---

## Step 3: Initialize TypeScript Configuration

Create a `tsconfig.json` file:

```bash
npx tsc --init
```

Now update the following options in `tsconfig.json`:

```json
{
  "compilerOptions": {
    "rootDir": "./src",
    "outDir": "./dist"
  }
}
```

> You can remove unnecessary comments from `tsconfig.json` for better readability.

---

## Step 4: Create Project Structure

Create the required folders:

```bash
mkdir src dist
```

Example structure:

```
project-name/
│── src/
│   └── index.ts
│── dist/
│── package.json
│── tsconfig.json
```

---

## Step 5: Write Your TypeScript Code

Create `src/index.ts`:

```ts
const message: string = "Hello TypeScript";
console.log(message);
```

---

## Step 6: Build the Project

Compile TypeScript to JavaScript:

```bash
npx tsc
```

This will generate compiled JavaScript files inside the `dist` folder.

---

## Step 7: Run the Project

Run the compiled JavaScript using Node.js:

```bash
node dist/index.js
```

---

## Optional: TypeScript Playground

You can experiment with TypeScript online using the official playground:

* [https://www.typescriptlang.org/play](https://www.typescriptlang.org/play)

---

## Summary

* Initialize project using `npm init -y`
* Install TypeScript as a dev dependency
* Configure `tsconfig.json`
* Write code inside `src/`
* Build using `npx tsc`
* Run using `node dist/index.js`


