# Getting Started With Schematics

This repository is a basic Schematic implementation that serves as a starting point to create and publish Schematics to NPM.

### Testing

To test locally, install `@angular-devkit/schematics-cli` globally and use the `schematics` command line tool. That tool acts the same as the `generate` command of the Angular CLI, but also has a debug mode.

Check the documentation with
```bash
schematics --help
```

### Unit Testing

`npm run test` will run the unit tests, using Jasmine as a runner and test framework.

### Publishing

To publish, simply do:

```bash
npm run build
// from the new repo link to the oughta-test schematic
npm link [directory]\oughta-test 
ng generate oughta-test:autospy src\app\tests --dry-run=false
ng generate oughta-test:oughta-test src\app\pages\shopping\shopping.component.ts --dry-run=false
// if the component already exists add --force at the end - if there are no meaningful tests in the .spec file
```

That's it!
 
