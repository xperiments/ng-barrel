# ng-barrel

Simple typescript barrel index file generator for the tree view.

## Usage

This utility add 2 context menu in the file navigation pane.

### Barrel Typescript

Barrel Typescript option will generate the barrel file for all the found typescript files excluding the .spec.ts files.

### Barrel All

Barrel All will generate a barrel index file of all the files inside the directory.

## Preventing overwriting custom code inside the barrel files

By default ng-barrel includes a // ng-barrel comment and puts all the resolved exports after this comment.
Code before the // ng-barrel comment will be preserved

    // Some comment to left inside our Code

    // ng-barrel

    export * from './demo-screen/demo-screen.component';
