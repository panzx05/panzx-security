# FlowFalcon Security

Security package sederhana untuk validasi user dan manajemen database bot.

## 🚀 Fitur
- Validasi username dan password
- Pendaftaran user baru
- Update database JSON langsung ke GitHub

## 📦 Instalasi
```bash
npm install flowfalcon-security
```
🔧 Penggunaan

Validasi User
```javascript
const { validateUser } = require('flowfalcon-security');

async function login() {
  try {
    const number = await validateUser('FlowFalcon', '1221');
    console.log(`Login berhasil untuk nomor: ${number}`);
  } catch (error) {
    console.error('Login gagal:', error.message);
  }
}

login();
```
Daftar User Baru
```javascript
const { registerUser } = require('flowfalcon-security');

async function register() {
  try {
    await registerUser('newUser', 'password123', '6281234567890');
    console.log('User berhasil terdaftar!');
  } catch (error) {
    console.error('Registrasi gagal:', error.message);
  }
}

register();
```
🐞 Laporan Bug

Laporkan bug di [Issues](https://github.com/FlowFalcon/flowfalcon-security/issues).

---
