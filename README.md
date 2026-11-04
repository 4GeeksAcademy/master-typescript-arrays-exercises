<!-- hide -->
<div align="center">

# Master TypeScript: Arrays

[![Certified tutorial](https://img.shields.io/badge/4Geeks_Academy-Certified_tutorial-2563eb)](https://4geeks.com/en/interactive-exercise)
[![Autograded with LearnPack](https://img.shields.io/badge/LearnPack-73_autograded_exercises-2563eb)](https://github.com/learnpack/learnpack)
[![Open in GitHub Codespaces](https://img.shields.io/badge/Open_in-GitHub_Codespaces-fb5a1f)](https://codespaces.new/4GeeksAcademy/master-typescript-arrays-exercises)

Read these instructions in [🇪🇸 Spanish](https://github.com/4GeeksAcademy/master-typescript-arrays-exercises/blob/HEAD/README.es.md)

</div>
<!-- endhide -->

Master TypeScript: Arrays is a LearnPack package with 74 exercise folders: a welcome screen plus 73 auto-graded challenges. You write every solution inside `app.ts`, and 442 Jest test cases check the value your function returns, never what you print. It covers array access, mutation versus copies, filtering, aggregation, numeric logic, matrices and binary search, with instructions in English and Spanish.

<!-- hide -->
## 📋 About this tutorial

- **Difficulty:** intermediate, as declared in `learn.json`; the first exercises are beginner level and the difficulty climbs steadily.
- **Exercises:** 74 folders, 73 of them with an automated test file.
- **Test cases:** 442 in total, between 3 and 14 per exercise, around 6 on average.
- **Technologies:** TypeScript 5.9, Node.js 22, Jest 29.7.0 and the LearnPack CLI.
- **Grading:** automatic and isolated per exercise, with `rewire` reading the functions inside your compiled file.
- **Languages:** every exercise ships with `README.md` and `README.es.md`.
<!-- endhide -->

## 🎯 What will you learn?

This package is pure practice on collections, one idea per exercise:

- **Indexed access:** reading the first, the last and the nth element, and what to return when the index does not exist.
- **Mutating versus copying:** `push`, `unshift`, `shift` and `pop` change the array you received; `slice`, `concat` and the spread operator build a new one. Four exercise pairs, eight exercises in total, exist precisely to make that difference obvious.
- **Filtering:** keeping only the elements that match a condition, and returning an empty array when nothing matches.
- **Transforming:** squaring every number, flattening arrays of arrays, joining two or three arrays into one.
- **Aggregating:** total, product, average, longest, shortest, largest and smallest, including arrays whose elements are of mixed types.
- **Strings as sequences:** counting characters, splitting a sentence into words or letters, collapsing double spaces, flipping characters in pairs.
- **Numeric logic without shortcuts:** rebuilding `%` and `*` from scratch, factorials, digit sums, compound interest and score-to-grade conversion.
- **Matrices:** reading `matrix[row][col]` safely and transposing rows into columns.
- **Search algorithms:** scanning a string character by character in `getIndexOf`, and binary search on a sorted array in the last two search exercises.
- **TypeScript in practice:** reading the typed signature you are given, working with `number[]`, `unknown[]`, `unknown[][]` and union return types such as `number | null`.

## 👀 What will you build?

73 small typed functions, one per folder, grouped in seven progressive blocks. 40 of them receive an array, 16 receive a string, 13 receive a number and 2 receive a matrix; the two left over take booleans (`or`) and objects (`extend`):

- **`001`–`012` Access, add and remove (12 exercises):** `getNthElement`, `getFirstElement`, `getLastElement`, `addToFront`, `addToBack`, `joinArrays`, `getElementsAfter`, `getElementsUpTo`, `removeFromFront`, `removeFromBack`, `removeFromFrontOfNew`, `removeFromBackOfNew`. Example: `getNthElement([1, 3, 5], 1)` returns `3`, and `getNthElement([], 3)` returns `undefined`.
- **`013`–`025` Words, comparisons and booleans (13 exercises):** `countCharacter`, `getAllLetters`, `getAllWords`, `or`, `extend`, `convertDoubleSpaceToSingle`, `areValidCredentials`, `getIndexOf`, `findMinLengthOfThreeWords`, `findMaxLengthOfThreeWords`, `repeatString`, `getLongestOfThreeWords`, `findShortestOfThreeWords`. Here you rebuild the `||` operator using only `!` and `&&`.
- **`026`–`033` Copies and filters (8 exercises):** `joinThreeArrays`, `addToFrontOfNew`, `addToBackOfNew`, `getAllElementsButNth`, `keep`, `removeElement`, `filterOddLengthWords`, `filterEvenLengthWords`. Example: `keep([1, 2, 3, 2, 1], 2)` returns `[2, 2]`, and `keep([1, 2, 1, 2, 1], 3)` returns `[]`.
- **`034`–`049` Aggregation and mixed arrays (16 exercises):** lengths of the longest and shortest element, `squareElements`, `filterOddElements`, `filterEvenElements`, `computeProductOfAllElements`, `computeSumOfAllElements`, `joinArrayOfArrays` and four functions that hunt for the smallest or largest number, and the shortest or longest word, inside arrays that also contain other types.
- **`050`–`063` Numeric logic (14 exercises):** `sum` and `average` together in one file, `calculateBillTotal`, `multiplyBetween`, `computeSumBetween`, `computeSummationToN`, `convertScoreToGrade`, `convertScoreToGradeWithPlusAndMinus`, `computeFactorialOfN`, `sumDigits`, `computeCompoundInterest`, `modulo`, `multiply`, `isOddWithoutModulo`, `isEvenWithoutModulo`.
- **`064`–`070` Algorithms on sequences (7 exercises):** `flipPairs`, `flipEveryNChars`, `detectOutlierValue`, `findPairForSum`, `isRotated`, `search`, `isIsogram`. Example: `detectOutlierValue("2 4 7 8 10")` returns `3`, the 1-indexed position of the only odd number.
- **`071`–`073` Matrices and binary search (3 exercises):** `getMatrixValue`, `transposeMatrix`, `binarySearchSortedArray`. Example: `transposeMatrix([[1, 2, 3], [4, 5, 6]])` returns `[[1, 4], [2, 5], [3, 6]]`, and `binarySearchSortedArray([1, 3, 5, 7, 9], 7)` returns `3`.

## 🎓 What do you need before starting?

- **JavaScript fundamentals:** variables, `if`, loops and how to call a function. The package starts at `arr[n]` and assumes you already got there.
- **No advanced TypeScript:** every `app.ts` arrives with the signature already typed, for example `function keep(arr: number[], keeper: number): number[]`. Your job is the body, not the type design.
- **Nothing installed if you use Codespaces:** the dev container sets up Node.js 22, Jest 29.7.0, the LearnPack CLI and the TypeScript plugin on its own.
- **Node.js if you work locally:** these are console programs, there is no browser, HTML or DOM anywhere in the package.

## ✅ How does the automatic grading work?

73 of the 74 folders contain a `test.js` file; only `00-Welcome`, the intro screen, has none. When you click `Test`, four things happen:

1. The LearnPack TypeScript plugin reads your `app.ts` and compiles it into `app.js` using the project `tsconfig.json` (target ES2019, CommonJS modules).

2. `rewire` loads that compiled `app.js` and pulls your function out of it **by its exact name**, with a line such as `const keep = rewire('./app.js').__get__('keep')`.

3. Jest 29.7.0 runs the assertions. All 73 files first check that the function exists, 69 also check that it returns something and 62 check the type of what comes back with `typeof`, before testing actual values.

4. Not a single one of the 442 test cases inspects the console. Every check calls your function and compares the returned value, so `console.log` is a debugging tool here, never the answer.

The same `learnpack audit` command runs on GitHub Actions with Node.js 22 on every push, which is why the exercise files stay consistent.

> 💡 Type errors do not fail your tests. The plugin transpiles your file rather than type-checking it, so only a syntax error stops the run. To get the full strict check, run `npm run typecheck`, which executes `tsc --noEmit` with `"strict": true`.

## 💡 What mistakes should you avoid?

1. **Printing instead of returning.** Zero tests read the console. If your function ends with `console.log(result)` and no `return`, it returns `undefined` and every assertion fails even though the output looks perfect.

2. **Editing `app.js` instead of `app.ts`.** The plugin regenerates `app.js` from `app.ts` on every Run and every Test, so anything you type directly into the JavaScript file is overwritten before it is graded.

3. **Renaming the function.** `rewire` looks it up by literal name, and in five exercises the folder name is not the function name: `045-joinArraysOfArrays` expects `joinArrayOfArrays`, `047-findSmallestnumberAmongMixedElements` expects `findSmallestNumberAmongMixedElements`, `050-averageIntegers` expects `sum` and `average`, `056-convertScoreToGradeWithPlus` expects `convertScoreToGradeWithPlusAndMinus` and `070-isogram` expects `isIsogram`. Trust the skeleton in `app.ts`, not the folder.

4. **Writing the banned operator in `060` and `061`.** Both tests read the compiled file as plain text and run a regular expression over it. `060 modulo` fails if a `%` appears anywhere, `061 multiply` fails if a `*` appears anywhere, comments included, so a leftover `/* ... */` block is enough to turn the exercise red.

5. **Solving `050` with a single function.** That file contains two skeletons, `sum` and `average`, and both are graded. The instructions also ask you to reuse the first one inside the second: `sum(arr) / arr.length`.

6. **Confusing the mutating twin with the copying one.** `004 addToFront` and `009 removeFromFront` work on the array you received; `027 addToFrontOfNew` and `011 removeFromFrontOfNew` must leave it untouched. The tests of `011` and `012` assert the input array afterwards: `removeFromFrontOfNew([9, 21, 74, 33])` has to return `[21, 74, 33]` while the input array still reads `[9, 21, 74, 33]`. `027` and `028` catch the same mistake from another angle, by requiring the returned array to be longer than the one you were given.

7. **Skipping the edge cases written in the instructions.** They are graded: an empty array returns `undefined` in `001`, `keep` returns `[]` when nothing matches, `getMatrixValue` returns `undefined` for a row or column that does not exist, and the two search exercises disagree on purpose, since `069 search` returns `null` when the value is missing while `073 binarySearchSortedArray` returns `-1`.

8. **Leaving the placeholder return.** Most skeletons ship with `return 0;`, `return '';`, `return false;` or `return [];` under the `// your code here` comment, and six of them arrive with no `return` at all. They exist so the file compiles, not as a valid answer.

## ❓ Frequently asked questions

### Do I need to know TypeScript before starting?

No, but you do need JavaScript. Every exercise hands you the typed signature already written, so you read types instead of designing them. You will get used to `number[]`, `string`, `unknown[]`, `unknown[][]` and union returns like `number | null` simply by filling in 73 function bodies. If you have never seen an annotation before, the [everyday types](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html) chapter of the official handbook is enough preparation.

### Can I solve the exercises with plain JavaScript inside `app.ts`?

Yes, and it will pass, because TypeScript is a superset of JavaScript and the plugin transpiles the file instead of type-checking it. You lose the point of the package though: the whole value is keeping the declared types honest. Run `npm run typecheck` at the root to see what strict mode thinks of your solutions.

### Why does my exercise fail when the console output is correct?

Because nothing is grading the console. The tests call your function with values you probably never tried, such as an empty array, a matrix index out of range or a negative number, and compare the returned value. Read the name of the failing assertion, it states the exact case that broke.

### Do I have to install anything to run it?

No, if you open the repository in [GitHub Codespaces](https://codespaces.new/4GeeksAcademy/master-typescript-arrays-exercises): the container installs Node.js 22, Jest 29.7.0, LearnPack and the TypeScript plugin, and the exercises open inside VS Code. [Gitpod](https://gitpod.io#https://github.com/4GeeksAcademy/master-typescript-arrays-exercises) is configured too. Locally you only need Node.js plus three commands.

### What is the difference between exercises `069` and `073`?

Both implement binary search on a sorted array, and both return the index when the value is found. The difference is the failure contract: `069 search` returns `null` when the value is not in the array, while `073 binarySearchSortedArray` returns `-1`. That is deliberate, since both conventions are common in real codebases and the tests check each one literally.

### Does it cost anything, and who owns the code I write?

The repository is public, so cloning it and solving the 73 exercises costs nothing, and the solutions you write inside `app.ts` are your own code. Note that this repository does not ship a `LICENSE` file, so no redistribution permission is granted for its content by default: if you want to republish or reuse the exercises themselves, ask 4Geeks Academy first.

<!-- hide -->
## 📚 Related tutorials

This package is part of the interactive TypeScript series and continues the JavaScript one:

1. [Fundamentals of TypeScript with Practice for JavaScript Developers](https://4geeks.com/en/interactive-exercise/fundamentals-of-typescript-with-practice-for-javas)
2. [Master TypeScript: Functions](https://github.com/4GeeksAcademy/master-typescript-functions-exercises), 42 auto-graded exercises
3. **Master TypeScript: Arrays** ← you are here
4. [Master TypeScript: Objects](https://github.com/4GeeksAcademy/master-typescript-objects-exercises), 55 auto-graded exercises

If arrays are still new to you, warm up with [Learn Javascript Arrays and Loops Interactive](https://4geeks.com/en/interactive-exercise/javascript-array-loops-exercises) and then come back.

## 🚀 How to start

The fastest way is [Open in GitHub Codespaces](https://codespaces.new/4GeeksAcademy/master-typescript-arrays-exercises). The container installs everything and VS Code opens the exercises for you.

If they do not start on their own, run this in the terminal:

```bash
learnpack start
```

You can also open the package in [Gitpod](https://gitpod.io#https://github.com/4GeeksAcademy/master-typescript-arrays-exercises). Use the top menu to move between exercises and to switch the instructions between English and Spanish.

## 💻 Local installation

Clone the repository and follow these steps, with Node.js already installed:

1. Install LearnPack globally:

    ```bash
    npm i @learnpack/learnpack -g
    ```

2. Install the TypeScript plugin that ships inside this repository:

    ```bash
    learnpack plugins:install file:$(pwd)/learnpack-typescript-plugin
    ```

3. Start the exercises from the same folder where `learn.json` lives:

    ```bash
    learnpack start
    ```

If something goes wrong, the [LearnPack quickstart for learners](https://4geeks.com/docs/learnpack/quickstart-for-learners) walks through the whole setup.

## 📚 How the exercises are organized

Each of the 73 exercise folders inside [`exercises/`](https://github.com/4GeeksAcademy/master-typescript-arrays-exercises/tree/HEAD/exercises) contains the same six files, with `00-Welcome` as the only exception, since it holds just the two READMEs:

- **`app.ts`:** the only file you edit. It arrives with the typed signature, a `// your code here` comment and an `export {}` at the bottom that turns the file into a module.
- **`app.js`:** the compiled output that LearnPack runs and Jest imports. It is regenerated from `app.ts` on every Run and Test.
- **`README.md`:** the instructions in English.
- **`README.es.md`:** the same instructions in Spanish.
- **`test.js`:** the Jest file that grades your solution. You do not need to open it, but reading it tells you exactly what is being asked.
- **`solution.hide.js`:** a working solution, hidden by LearnPack until you ask for it.

The repository root also holds `tsconfig.json` with `"strict": true` and the npm scripts `typecheck`, `audit:signatures`, `regenerate:app-ts` and `transpile:all`, used to keep the 73 skeletons and their tests in sync.

## 🤝 Contributors

- [Ehiber Graterol (ehiber)](https://github.com/ehiber): the only contributor in the repository history, author of the exercises, their tests and the LearnPack TypeScript plugin.
- According to [CHANGELOG.md](https://github.com/4GeeksAcademy/master-typescript-arrays-exercises/blob/HEAD/CHANGELOG.md), the first batches of exercises this package is based on were written by Mike Berrio.

See the full list on the [contributors graph](https://github.com/4GeeksAcademy/master-typescript-arrays-exercises/graphs/contributors). Contributions of any kind are welcome: if you find a bug or a typo in an exercise, please open an issue or send a pull request.
<!-- endhide -->
