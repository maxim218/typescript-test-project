# TypeScript test project

Устанавливаем глобально TypeScript

```
sudo npm install -g typescript
```

Смотрим версию TypeScript

```
tsc --version
```

Создаем файл tsconfig.json и пишем в нем

```
{
    "compilerOptions": {
      "target": "es5",
      "module": "commonjs",
      "sourceMap": true
    }
}
```

Создаем файл programA.ts и пишем в нем

```
let myStringFirst: string = "hello";
console.log(myStringFirst);

let myStringSecond: string = "world";
console.log(myStringSecond);
```

Запускаем перевод из TypeScript в JavaScript

```
tsc programA.ts
```

После автоматического создания файла programA.js запускаем его

```
node programA.js
```
