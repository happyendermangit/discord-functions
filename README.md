# Discord Functions
✨A database of discord functions and how to find them using a string, useful for dataminers.✨

## Why i made this?
Discord pushed an update to their client which renamed about every exports names, so i'm creating this so that you can still use these functions with their name

## 🚀 | Contributing:

- I'm looking for contributors, if you want to help, here is the info:

1. there is 2644 functions left from the old build
2. please avoid making the find_with use Endpoints.something because Endpoints isnt a valid export on the new build
3. [here you can find the old functions](https://github.com/happyendermangit/discord-functions/blob/main/need_to_do_functions.json)
Example function:
```json
{
  "name": "camelCaseName",
  "find_with":"String That Will Never Change and is only on this function",
  "method": "findFunctionByCode"
}
```

## How to use this data:

Here is some typescript types that explains the data structure
```ts
interface Function {
 name: string;
 find_with: string;
 method: "findFunctionByCode"
}
type Chunk = Function[]
type FunctionsNames = Chunk[]
```

If you cant read these typescripts types, here is the structure of the data:
- The chld elements of the array are the chunks, these chunks contain the their functions with their name, find_with and method
