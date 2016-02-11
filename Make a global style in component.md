### How to make a global style in component 
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
