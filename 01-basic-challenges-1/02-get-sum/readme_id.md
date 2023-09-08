# Tantangan: Dapatkan Jumlah

Ini adalah tantangan latihan yang sangat dasar lagi hanya untuk membuat Anda terbiasa.

## Petunjuk

Buatlah sebuah fungsi yang disebut `getSum` yang mengambil dua angka dan mengembalikan jumlah dari kedua angka tersebut.

### Tanda Tangan Fungsi

```js
/**
 * Mengembalikan jumlah dari dua angka.
 * @param {number} a - Angka pertama.
 * @param {number} b - Angka kedua.
 * @returns {number} - Jumlah dari dua angka tersebut.
 */
function getSum(a: number, b: number): number;
```

### Contoh

```JS
getSum(1, 2) // 3
getSum(10, 5) // 15
getSum(2, 2) // 4
getSum(10, 5) // 15
```

### Batasan

- Fungsi harus mengembalikan angka

### Petunjuk

- Anda dapat menggunakan operator `+` untuk menjumlahkan dua angka.

## Solusi

<details>
  <summary>Klik Untuk Solusi</summary>

```JS
function getSum(a, b) {
  return a + b;
}
```

### Penjelasan

Ini adalah tantangan yang cukup sederhana. Kami membuat sebuah fungsi yang mengambil dua nilai dan kami menjumlahkan dua nilai tersebut. Kemudian kami mengembalikan hasil penjumlahan dua nilai tersebut.

</details>

### Kasus Uji

```JS
test('Menghitung jumlah dua angka', () => {
  // Input kasus uji
  const num1 = 5;
  const num2 = 7;

  // Panggil fungsi
  const result = getSum(num1, num2);

  // Periksa apakah hasilnya sama dengan jumlah yang diharapkan
  expect(result).toBe(12);
});
```
