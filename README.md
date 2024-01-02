# AngularFirebaseKanban

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 17.0.8.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.

https://developers.google.com/codelabs/building-a-web-app-with-angular-and-firebase#0 from October 10, 2023.

 ng new angular-firebase-kanban --no-strict --no-standalone --routing=false --style=css
 , Do you want to enable Server-Side Rendering (SSR) and Static Site Generation (SSG/Prerendering)? No, open folder, see: no app.routes.ts, no app.config.ts, no app.config.server.ts ,

 "1. Introduction
 2. Creating a new project
 3. Adding Material and the CDK
 4. Visualizing tasks
 5. Implementing drag and drop for tasks
 6. Creating new tasks
 7. Improving the app's styles
 8. Editing and deleting existing tasks
 9. Creating a new Firebase project
 10. Adding Firebase to the prject
 11. Moving the data to Firestore
 12. Improving optimistic updates
 13. Deploying the application
 14. Congratulations"

 ng add @angular/material, theme= indigo-pink,
 app.component.html: add a toolbar,
app.module.ts: import MatToolbarModule and
    MatIconModule, import { MatToolbarModule } from '@angular/material/toolbar';
import { MatIconModule } from '@angular/material/icon'; , 
ng s -o to see the Kanban Fire toolbar in browser, 
Step2. ng g c task --skip-tests, then make task.ts file: export interface,
task.component.ts: input, output, eventemitter, edit, import Task from task.ts, task.component.html: ngIf, string interpolation, edit, emit,
app.module.ts: import MatCardModule, 
app.component.ts: define an array and add tasks, import Tasks, app.component.html: use ngFor, look at page in browser,
5. implementing drag and drop: 
app.component.html: remove ngFor and add 3 swimlanes, app.module.ts: import DragDropModule, app.component.ts: declare inProgress, done, editTask, drop methods,
import { CdkDragDrop, transferArrayItem } from '@angular/cdk/drag-drop';
ng s -o to see if results look right,
6. creating new tasks: app.component.html: add button between toolbar and swimlanes div, app.module.ts: import { MatButtonModule } from '@angular/material/button'; , app.component.ts: import { MatDialog } from '@angular/material/dialog'; , app.module.ts: import { MatDialogModule } from '@angular/material/dialog'; , now: ng g c task-dialog --skip-tests, task-dialog.component.html: modal content, task-dialog.component.ts: inject, matdialogdata, matdialogref, task, backuptask, cancel, task-dialog.component.ts: export interfaces taskdialogdata and taskdialogresult, 
app.module.ts: import  MatInputModule,
    FormsModule, app.component.ts: import taskdialogcomponent and taskdialogresult, ng s -o,
    7. improve the app's styles (CSS): app.component.css,
    task.component.css, 
    8. editing and deleting existing tasks: task-dialog.component.html: add a delete button, app.component.ts: replace editTask, https://github.com/FirebaseExtended/codelab-kanban-fire/tree/editing-and-deleting-existing-tasks , 
    

