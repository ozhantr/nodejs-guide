# Non-Blocking I/O in Action

Node.js shines in I/O-heavy workloads because of **non-blocking** behavior.

## 🧪 Blocking vs Non-Blocking:

```js
// Blocking (bad)
const data = fs.readFileSync('file.txt');
console.log(data);

// Non-blocking (good)
fs.readFile('file.txt', (err, data) => {
  console.log(data);
});
```

- **Blocking**: CPU waits until task completes.
- **Non-blocking**: Task is delegated, CPU keeps working.

## ⚡ Result:

- Minimal CPU idle time
- High concurrency
- Efficient use of resources
