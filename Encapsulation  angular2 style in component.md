### How to make a global style in component (ViewEncapsulation.None)
global style in and component style out
```typescript
import {ViewEncapsulation} from 'angular2/core';

@Component({
    ...
    encapsulation: ViewEncapsulation.None,
    ...
    template:<style>
                .completed{
                    some-style: line-through;
                }
            </style>
})
```
### How to make global style don't into component (ViewEncapsulation.Native)
global style don't in and component style dont'
```typescript

@Component({
    ...
    encapsulation: ViewEncapsulation.Native,
    ...
  
})
```
###default (ViewEncapsulation.Emulatedve)
global style  in and component style dont' out
```typescript

@Component({
    ...
    encapsulation: ViewEncapsulation.Emulatedve,
    ...
  
})
```
