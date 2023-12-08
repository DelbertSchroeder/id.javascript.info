
Kamu bisa perhatikan berikut:

```js no-beautify
function pow(x,n)  // <- tak ada spasi diantara arguments
{  // <- menemukan bracket di baris terpisah
  let result=1;   // <- tak ada spasi sebelum atau setelah =
  for(let i=0;i<n;i++) {result*=x;}   // <- tak ada spasi
  // konten { ... } sebaiknya di baris baru
  return result;
}

let x=prompt("x?",''), n=prompt("n?",'') // <-- secara teknis bisa saja
// tapi akan lebih baik jika dibuat dua baris, juga jangan gunakan spasi dan jangan lupa tanda ;
if (n<=0)  // <- tidak ada spasi didalam (n <= 0), dan harus ada baris tambahan diatasnya
{   // <- pembuka kurung kurawal di baris baru
  // dibawah - baris yang panjang dapat dibagi menjadi beberapa baris untuk menambah keterbacaan kode
  alert(`Power ${n} is not supported, please enter an integer number greater than zero`);
}
else // <- bisa menulisnya di baris tunggal seperti "} else {"
{
  alert(pow(x,n))  // tak ada spasi dan kehilangan ;
}
```

Varian yang dibetulkan:

```js
function pow(x, n) {
  let result = 1;

  for (let i = 0; i < n; i++) {
    result *= x;
  }

  return result;
}

let x = prompt("x?", "");
let n = prompt("n?", "");

if (n <= 0) {
  alert(`Power ${n} is not supported,
    please enter an integer number greater than zero`);
} else {
  alert( pow(x, n) );
}
```
