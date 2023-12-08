nilai penting: 4

---

# Tulis ulang fungsi menggunakan '?' atau '||'

Fungsi berikut mengembalikan nilai `true` jika parameter `age` lebih besar daripada `18`.

Jika tidak, fungsi akan meminta sebuah konfirmasi dan mengembalikan nilainya.


```js
function checkAge(age) {
  if (age > 18) {
    return true;
  } else {
    return confirm('Did parents allow you?');
  }
}
```

Tulis ulang fungsi, untuk melakukan dengan sama, tetapi tanpa `if`, dalam satu baris.

Buatlah dua variasi dari `checkAge`:

1. Menggunakan sebuah tanda tanya operator `?`
2. Mengguunakan OR `||`
