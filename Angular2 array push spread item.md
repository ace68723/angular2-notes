instade of use
```typescript
  Array.push(item);
```
we use
```typescript
  this.array = [...this.todos, item];// copy all over the old array and add a new item 
```
