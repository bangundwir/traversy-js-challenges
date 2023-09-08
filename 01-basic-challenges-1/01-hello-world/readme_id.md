# Tantangan: Contoh Tantangan Hello World

Ini adalah tantangan latihan untuk menunjukkan kepada Anda bagaimana hal-hal disusun dan cara menguji, dll.

## Petunjuk

Buatlah sebuah fungsi yang disebut `helloWorld` yang mengembalikan string 'Hello World!'.

### Tanda Tangan Fungsi

```js
/**
 * Mengembalikan string yang berisi 'Hello World!'.
 * @returns {string} - String 'Hello World!'.
 */
function helloWorld(): string;
```

### Contoh

```JS
helloWorld() // 'Hello World!'
```

### Batasan

Saya akan menentukan batasan-batasan di sini. Batasannya akan bervariasi tergantung pada tantangannya.

- Fungsi harus mengembalikan string

### Petunjuk

- Saya akan memberikan beberapa petunjuk di sini. Anda bisa memilih untuk menggunakannya atau tidak.

## Solusi

<details>
  <summary>Klik Untuk Solusi</summary>

```JS
function printHelloWorld() {
  return 'Hello World!';
}
```

### Penjelasan

Saya akan memberikan penjelasan solusi di sini. Panjang dan kedalaman penjelasannya akan bervariasi tergantung pada tantangannya.

</details>

### Kasus Uji

Uji Jest akan ditempatkan di sini. Mereka sudah termasuk dalam berkas kursus. Anda hanya perlu menjalankan `npm test`. Terkadang saya juga akan menambahkan uji manual di sini.

```JS
test("Mengembalikan 'Hello, World!' sebagai string", () => {
  const result = helloWorld();
  expect(result).toBe('Hello World!');
});
```
