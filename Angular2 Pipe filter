### Pipe filter

```typescript
import {Injectable, Pipe} from 'angular2/core';

@Pipe({
  name: 'search'
})
@Injectable()
export class SearchPipe {
  transform(value, args) {
        
        return value.filter((item) => item.title.startsWith('A'))
  }
```
```typescript 
import {Component} from 'angular2/core';
import {SearchPipe} from '/search-pipe';
@Component({
    selector: 'todo-list',
    pipes: [SearchPipe]
    template:   '<button>Primary</button>'+
                '<ul>'+
                    '<li *ngFor="#todo of todoService.todos | search">'+
                        '<todo-item-renderer [todo]="todo"></todo-item-renderer>'+
                    '</li>   '+ 
                '</ul>',
    directives: [IONIC_DIRECTIVES,TodoItemRenderer]  
})
export class TodoList {
  constructor(public todoService:TodoService) {
    this.text = 'Hello World';
    console.log(todoService.todos)
  }
}
```
