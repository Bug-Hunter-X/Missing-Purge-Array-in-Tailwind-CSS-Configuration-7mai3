# Missing Purge Array in Tailwind CSS Configuration

This repository demonstrates a common error in Tailwind CSS configuration:  a missing or improperly configured `purge` array in the `tailwind.config.js` file.

## The Problem

The `purge` option in the Tailwind CSS configuration file tells Tailwind which files to scan for class names. If this array is missing or empty, Tailwind will not remove unused CSS classes, leading to larger CSS files and potential performance issues.

## The Solution

The solution is to properly configure the `purge` array in your `tailwind.config.js` file. This array should contain the paths to your templates or components.   The specific paths will depend on your project setup (e.g., Next.js, Vue.js, etc.).  Consult the Tailwind CSS documentation for the most up-to-date instructions.

## How to reproduce the bug
1. Clone this repository.
2. Notice the `tailwind.config.js` file has no purge array.
3. Run `npm install` (if needed)
4. You will likely notice unexpected behavior with Tailwind CSS.

## How to fix the bug
1. Modify `tailwind.config.js` as in `tailwind.config.solution.js` file
2. Rerun your build process.