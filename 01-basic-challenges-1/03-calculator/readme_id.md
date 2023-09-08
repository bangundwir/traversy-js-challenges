# Tantangan: Kalkulator

## Petunjuk

Buatlah sebuah fungsi yang disebut `kalkulator` yang mengambil 2 angka dan sebuah operator, dan mengembalikan hasil perhitungan.

### Tanda Tangan Fungsi

```js
/**
 * Mengembalikan hasil perhitungan.
 * @param {number} num1 - Angka pertama.
 * @param {number} num2 - Angka kedua.
 * @param {string} operator - Operator yang akan digunakan dalam perhitungan.
 * @returns {number} - Hasil perhitungan.
 */
function kalkulator(num1: number, num2: number, operator: string): number;
```

### Contoh

```JS
kalkulator(1, 2, '+') // 3
kalkulator(10, 5, '-') // 5
kalkulator(2, 2, '*') // 4
kalkulator(10, 5, '/') // 2
```

### Batasan

- Fungsi harus mengembalikan angka.
- Fungsi harus melempar atau mencatat kesalahan jika operator yang tidak valid diberikan.

### Petunjuk

- Anda dapat menggunakan pernyataan `if` atau pernyataan `switch` untuk menentukan operator yang diberikan.

## Solusi

<details>
  <summary>Klik Untuk Solusi 1</summary>

#### Menggunakan pernyataan `switch`:

```js
function kalkulator(num1, num2, operator) {
  let hasil;

  switch (operator) {
    case '+':
      hasil = num1 + num2;
      break;
    case '-':
      hasil = num1 - num2;
      break;
    case '*':
      hasil = num1 * num2;
      break;
    case '/':
      hasil = num1 / num2;
      break;
    default:
      throw new Error('Operator tidak valid');
  }

  return hasil;
}
```

### Penjelasan

- Membuat sebuah fungsi yang disebut `kalkulator` yang mengambil tiga argumen: `num1`, `num2`, dan `operator`.
- Membuat variabel `hasil` untuk menyimpan hasil perhitungan.
- Menggunakan pernyataan `switch` untuk menentukan operator yang diberikan. Jika itu +, -, \*, atau /, kami melakukan perhitungan. Jika operatornya adalah yang lain, kami melempar sebuah kesalahan.

</details>

<details>
 <summary>Klik Untuk Solusi 2</summary>

#### Menggunakan pernyataan `if`:

```js
function kalkulator(num1, num2, operator) {
  let hasil;

  if (operator === '+') {
    hasil = num1 + num2;
  } else if (operator === '-') {
    hasil = num1 - num2;
  } else if (operator === '*') {
    hasil = num1 * num2;
  } else if (operator === '/') {
    hasil = num1 / num2;
  } else {
    throw new Error('Operator tidak valid');
  }

  return hasil;
}
```

### Penjelasan

- Membuat sebuah fungsi yang disebut `kalkulator` yang mengambil tiga argumen: `num1`, `num2`, dan `operator`.
- Membuat variabel `hasil` untuk menyimpan hasil perhitungan.
- Menggunakan pernyataan `if` untuk menentukan operator yang diberikan. Jika itu +, -, \*, atau /, kami melakukan perhitungan. Jika operatornya adalah yang lain, kami melempar sebuah kesalahan.

 </details>

### Kasus Uji

```js
test('Melakukan operasi aritmatika menggunakan fungsi kalkulator', () => {
  // Input kasus uji
  const num1 = 5;
  const num2 = 7;

  // Penambahan
  expect(kalkulator(num1, num2, '+')).toBe(12);

  // Pengurangan
  expect(kalkulator(num1, num2, '-')).toBe(-2);

  // Perkalian
  expect(kalkulator(num1, num2, '*')).toBe(35);

  // Pembagian
  expect(kalkulator(num1, num2, '/')).toBeCloseTo(0.7143, 4);

  // Operator tidak valid
  expect(() => kalkulator(num1, num2, '^')).toThrow('Operator tidak valid');
});
```
