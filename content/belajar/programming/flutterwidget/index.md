---
title: "Widget Flutter"
date: 2023-06-19T16:12:30+08:00
draft: false

showtableofcontents: true
tags: ["Mobile Developer", "Flutter", "Widget", "Dart", "Dasar Flutter"]

series: ["Mobile Developer"]
series_order: 5
---

<h2>Widget Flutter</h2>

- Text Widget
- Column & Row Widget
- Container Widget
- Stateless & Statefull Widget

<h2>Method</h2>

- Anonymous Method

## Text Widget

### Parameter

Parameter pada text widget :

- maxLines
- overflow
- softWrap
- textAlign

```dart
body: Center(
   child: Container(
     color: Colors.amber,
     width: 150,
     height: 150,
     child: const Text(
       'hai kami sedang belajar dasar widget flutter menggunakan visual studio code dan virtual device',
       maxLines: 2,
       overflow: TextOverflow.e ellipsis,
       softWrap: false,
       textAlign: TextAlign. justify,
        ), // Text
    ), // Container
), // Center
```

### Text Style

Text Style parameter :

- color
- fontSize
- fontWeight
- backgroundColor
- fontStyle

```dart
body: Center(
    child: Container(
        color: Colors.amber,
        width: 150,
        height: 150,
        child: const Text(
            'hai kami sedang belajar dasar widget flutter menggunakan visual studio code dan virtual device',
            style: TextStyle(
            color: Colors.white,
            fontSize: 15,
            fontWeight: FontWeight.w700,
            backgroundColor: Colors.black,
            fontStyle: FontStyle. italic,
            ), // TextStyle
        ), // Text
    ), // Container
), //Center

```

## Column & Row

- Column : Vertical
- Row : Horizontal

```dart
body: const Column(
  mainAxisAlignment: MainAxisAlignment. center,
  crossAxisAlignment: CrossAxisAlignment. start,
   children: [
    Text ("Data 1"),
    Text ("Data 2"),
    Text ("Data 3"),
    Text ("Data 4"),
     Row(
       children: [
         Text ("Data 1"),
         Text ("Data 2"),
         Text ("Data 3"),
         Text ("Data 4"),
         Text ("Data 5")
       ],
        ), // Row
    ],
), //Column

```

## Container Widget

### Padding & Margin

Padding : Mengatur jarak dalam.

Margin : Mengatur jarak luar.

Properti Edge.Insets :

- all()
- fromLTRB()
- only()
- symmetric().

```dart
body: Container(
  margin: const EdgeInsets.all(10),
  padding: const EdgeInsets.all(60),
  color: Colors.amber,
  child: Container(
    color: Colors.black,
  ),// Container
),// Container
```

### BoxDecoration

Untuk styling container

```dart
body: Center(
    child: Container(
        decoration: BoxDecoration(
            color: Colors.black,
            borderRadius: BorderRadius.circular(10),
            border: Border.all(color: Colors.white, width: 10),
            gradient: const LinearGradient(
            colors: [Colors.pink, Colors.black],
            begin: Alignment.bottomCenter,
            end: Alignment.topCenter,
            ), // LinearGradient
        ), // BoxDecoration
    ), // Container
),

```

## Stateless & Stateful

### StatelessWidget

Stateles tidak memiliki perubahan pada tampilan atau tampilannya fixed. Tidak
ada perubahan lagi dari user.

StatelessWidget contohnya seperti dibawah ini :

```dart
class MainApp extends StatelessWidget {
  const MainApp({super.key});

  @override
  Widget build(BuildContext context) {
    return const MaterialApp(
      home: Scaffold(
        body: Center(
          child: Text("Berkah IT"), // Container
        ),
      ),
    );
  }
}
```

### StatefulWidget

StatefulWidget biasa kita gunakan jika ada data yang dinamis (dapat berubah
ketika user melakukan sebuah aksi). Seperti perhitungan angka atau animasi dalam
aplikasi.

StatefulWidget memiliki tanda State. Seperti dibawah ini :

```dart
class MainApp extends StatefulWidget {
  const MainApp({super.key});

  @override
  State<MainApp> createState() => _MainAppState();
}

class _MainAppState extends State<MainApp> {

}
```

Contoh aplikasi sederhana penggunaan StatefulWidget :

```dart
class _MainAppState extends State<MainApp> {
  int angka = 0;

  void tambahBilangan() {
    setState(() {
      angka++;
    });
  }

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: const Text("Berkah IT"),
        ),
        body: Center(
          child: Column(
            children: [
              Text("Angka ke $angka"),
              ElevatedButton(
                onPressed: () {
                  tambahBilangan();
                },
                child: const Text("Tambah"),
              ),
            ],
          ),
        ),
      ),
    );
  }
}

```

## Anonymous Method

Anonymous Method merupakan method yang tidak memiliki nama. Penempatannya
langsung di dalam fungsi. Seperti contoh di bawah ini :

```dart {linenos=table,hl_lines=[9,"24-27"],linenostart=1}
class MainApp extends StatefulWidget {
  const MainApp({super.key});

  @override
  State<MainApp> createState() => _MainAppState();
}

class _MainAppState extends State<MainApp> {
  int angka = 0;

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
         appBar: AppBar(
          title: const Text("Berkah IT"),
        ),
        body: Center(
          child: Column(
            children: [
              Text("Angka ke $angka"),
              ElevatedButton(
                onPressed: () {
                  setState(
                    () {
                      angka++;
                    }, // Anonymous Method
                  );
                },
                child: const Text("Tambah"),
              ),
            ],
          ),
        ),
      ),
    );
  }
}

```
