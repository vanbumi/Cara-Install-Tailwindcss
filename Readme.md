# Cara Install Tailwindcss

Masih banyak developer pemula yang kesulitan untuk meng-install Tailwindcss karena Update commands instalasi dari web Tailwindcss.com.

Source: https://tailwindcss.com/docs/installation

## Persiapan

- Pertama-tama buatlah folder proyek yang akan anda bangun, berinama project sesuai yang anda inginkan.
  Misalnya tailwind_app

- Buka folder tailwind_app dengan menggunakan Code Editor, misalnya Visual Code Studio.

- Buka Integrated Terminal di Visual Code Studio. Kemudian lakukan setup seperti dibawah ini:

## Create your configuration file

```
npx tailwindcss init
```

Untuk membuat file tailwind.config.js pada root project anda.

## Initial Project

```
npm init

atau

npm init -y
```

untuk men-generate file package.json

## Install Tailwind via npm

```
npm install tailwindcss@latest postcss@latest autoprefixer@latest
```

Otomatis akan men-generate folder node_modules

## Membuat folder src pada root project.

```
mkdir src
```

## Buat file css dibawah folder css

```
src/style.css
```

## Tambahkan sintax tailwind di file style.css

```
// src/style.css

@tailwind base;
@tailwind components;
@tailwind utilities;
```

## Tambahkan baris code ini pada file package.json

Pada property "scripts" diatas "test":, menjadi:

```
"build:css": "tailwindcss build src/style.css -o dist/style.css",
"test": "echo \"Error: no test specified\" && exit 1"
```

## Run build

```
npm run build:css
```

bila sukses build akan muncul seperti dibawah ini:

tailwindcss 2.0.2

🚀 Building: src/style.css

✅ Finished in 6.48 s
📦 Size: 3.74MB
💾 Saved to dist/style.css

Semoga membantu :)
